# Table tests

This template gives you the boilerplate to create table tests.

Suggested abbreviation: `tt`

```
cases := []struct {
	name string
	in $IN_TYPE$
	want $OUT_TYPE$
}{
	{
		name: `$NAME$`,
		in: $INPUT$,
		want: $WANTED_VALUE$,
	},
}

for _, tt := range cases {
	t.Run(tt.name, func(t *testing.T) {
		
		got := $THING_UNDER_TEST$(tt.in)
		
		if got != tt.want {
            t.Errorf(`$THING_UNDER_TEST$(%v) = %v; want "%v"`, tt.in, got, tt.want)
    }
    
	})
}
```

## References

[Code Review Comments#useful-test-failures](https://github.com/golang/go/wiki/CodeReviewComments#useful-test-failures)

## Demo

[![Demo of table test live template](http://img.youtube.com/vi/2oaEGnNqwTs/0.jpg)[View on YouTube](https://www.youtube.com/embed/2oaEGnNqwTs)]

## Hat tips 

[Contributors from this gist](https://gist.github.com/bwplotka/a151fe43c9851ef092d29f912e7f8ca7)
