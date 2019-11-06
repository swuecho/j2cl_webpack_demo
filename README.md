# j2cl_webpack_demo

## how this project is created?

1. This probject is created using `vue create j2cl_webpack_demo` 
2. The `helloworld.js` and `helloword.js` is copied from j2cl sample project with minor modification. [j2cl_export_symbol_demo](https://github.com/swuecho/j2cl_export_symbol_demo). These two files are included in the git repo. (copied from bazel-bin/src folder after run `bazel build`)

3. after `yarn install` and `yarn serve`, the output in the sceen should be 'Hello from Java! and JS!'
![hello](/public/j2cl_hello.png)


# why this useful?

If you have a java lib and want to use it in browser, you can use this approach. 

How about start a new project and write new code in java? You will have better experience with other language, such as typescript, bucklescript.



