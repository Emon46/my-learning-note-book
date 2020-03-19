# macaron-demo

## creates and returns a Classic Macaron.
```go
m := macaron.Classic()
```
## macaron.classsic() auto generate
```
Request/response logging - macaron.Logger
Panic recovery - macaron.Recovery
Static file serving - macaron.Static
```
## macron handler workflow
```
https://go-macaron.com/core_concepts#handler-workflow
```
## context.next()
Method Context.Next is an optional feature that Middleware Handlers can call to yield the until after the other Handlers have been executed.
This works really well for any operations that must happen after an HTTP request

---
---
---
# ISSUES
## dummy render not register
```go
	m.Use(macaron.Renderer())
  ```
  if there is no  middleware to render
