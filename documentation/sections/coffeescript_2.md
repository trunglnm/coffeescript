## CoffeeScript 2

CoffeeScript 2 generates JavaScript that uses the latest ES2015+ features. It is your responsibility to ensure that your target JavaScript runtime(s) support all these features, or that you pass the output through another transpiler like [Babel](http://babeljs.io/), [Rollup](https://github.com/rollup/rollup) or [Traceur Compiler](https://github.com/google/traceur-compiler). In general, [CoffeeScript 2’s output is fully supported by Node.js 7+](http://node.green/), although async functions require the `--harmony` or `--harmony-async-await` flags; and ES2015 modules require an additional transpiler. Output JavaScript intended for browsers generally requires additional transpilation.

If you’re looking for a single tool that takes CoffeeScript input and generates JavaScript output that runs in any JavaScript runtime, assuming you opt out of certain newer features, stick to the [CoffeeScript 1.x branch](v1/). CoffeeScript 2 [breaks compatibility](#breaking-changes) with certain CoffeeScript 1.x features in order to conform with the ES2015+ specifications, and generate more idiomatic output (a CoffeeScript `=>` becomes an ES `=>`; a CoffeeScript `class` becomes an ES `class`; and so on).