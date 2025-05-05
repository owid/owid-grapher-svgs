# owid-grapher-svgs

_Reference data and generated images for comparison._

This repo contains a reference set of static grapher configs and data that can be used alongside the `svgTester` tools in the [owid-grapher](https://github.com/owid/owid-grapher) repo.

## How to use

Use this manually when you have changed grapher, and want to know if your change has changed any chart layouts.

1. Clone the repo locally, in a sibling folder to `owid-grapher`.
2. Regenerate any SVGs that have changed

    ```
    yarn tsx --tsconfig tsconfig.tsx.json devTools/svgTester/export-graphs.ts \
        -i ../owid-grapher-svgs/configs \
        -o ../owid-grapher-svgs/svg
    ```

3. Use git to see any changes
4. If there are changes, commit them to a branch and you can see a visual diff on Github
