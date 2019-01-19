# Web server

Suggested abbreviation: `webserver`

This template can be run inside an empty Go file to create a simple web server.

## Notes

This takes care of some of the tedium of creating the TCP network address from a port number and properly reports an error if the server cannot be started.

```
package main

import (
	"fmt"
	"log"
	"net/http"
)

func helloWorld(w http.ResponseWriter, r *http.Request) {
	fmt.Fprint(w, "Hello, world")
}

func main() {
	port := "5000"

	router := http.NewServeMux()
	router.HandleFunc("/", helloWorld)

	log.Printf("trying to listen on port %s", port)

	if err := http.ListenAndServe(fmt.Sprintf(":%s", port), router); err != nil {
		log.Fatalf("unable to listen on port %s, %+v", port, err)
	}
}
```