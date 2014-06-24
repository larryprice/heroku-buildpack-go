heroku-buildpack-go
===================

Opinionated buildpack for GO web applications

#Usage

Place a .goconfig file at the root of your proyect with the package path, like:

```
github.com/jarias/myawesomeapp
```

The build should use make and have a **stage** task that would be executed by the buildpack this task should take care of getting dependencies and building your app using any tool you like a simple `go get` and `go build` or a tool like [gpm](https://github.com/pote/gpm), [gox](https://github.com/mitchellh/gox), [goxc](https://github.com/laher/goxc), etc, your app executable should be output into an **out** directory a the root of the project.

#Acknowledgement

Work is based of Keith Rarick GO buildpack (https://github.com/kr/heroku-buildpack-go)

#LICENSE

Copyright 2014 Julio Arias

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
