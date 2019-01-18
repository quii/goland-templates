# Table tests

This template gives you the boilerplate to create table tests.

`tt`

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
            t.Errorf(`$THING_UNDER_TEST$(%v) = %v; want %v`, tt.in, got, tt.want)
    }
    
	})
}
```

## References

[Code Review Comments#useful-test-failures](https://github.com/golang/go/wiki/CodeReviewComments#useful-test-failures)

## Demo

todo

