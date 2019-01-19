# GoLand templates

[GoLand](https://www.jetbrains.com/go/) is an IDE for Go developers and this project lists useful templates for common tasks for developers to speed up their days and write consistent code. 

It's hoped that this project can be a discussion point for building a solid list of idiomatic templates.

## Contents

- [Table tests](table-tests.md)

## What?

When you type `main` and hit return in GoLand it will create some code for you.

```go
func main() {
	
}
```

GoLand has many templates built in. To see them double press shift, type "live templates" and hit return to see the preferences. From there you can see a listing of templates available to you like `test`.

```go
func TestName(t *testing.T) {
	
}
```

GoLand lets you add your own live templates and the hope is this repository will be a community driven curation of templates that adhere to Go's best practices. 

## Why?

A lot of developers like to talk about developer productivity in terms of being able to create code very quickly by honing their skills with their editor/IDE of choice. 

I don't entirely subscribe to this view. Typing is very incidental to software development. It is a _thinking_ profession and we dont spend 8 hours a day constantly typing, racing our colleagues to see who can write the most code.

However _consistency_ is a very valuable trait not only within a particular code base but a whole community. This I feel is something that Go gets right. With a deliberately limited syntax there's only so many ways a developer can solve problems, especially compared to other programming languages. 

With the excellent, backward-compatible standard library which lets Go developers solve many problems with well documented and known functions Go has the opportunity to have code that everyone can recognise and understand at a glance. 

For ideas as to what the Go community feels like are standards take a look at [Go Code Review Comments](https://github.com/golang/go/wiki/CodeReviewComments).

As software developers _we can extend our tooling_ to help us bring more consistency to our software to help us all be more productive and the intention of this project is to help facilitate that. 

## How can I contribute?

The usual: PR's, issues, etc. 

Submitting your own templates would be fantastic. Try and follow the general structure of [Table tests](table-tests.md) so readers get an explanation of what it's for. 