# How to use

1. Git clone the CRE CLI into a different directory and run the build command specified in the CLI's README so that you have the `cre` executable in that project's root. For me the `cre` cli executable is in `"/Users/zubinpratap/code/cre-cli/`

2. `pnpm install` to install the dependencies of this examples project.

3. In this projects root, open terminal and alias cre to point the cre executable. For me it looks like
   `alias cre="/Users/zubinpratap/code/cre-cli/cre"`

4. set copy `.env.example` into a `.env` file with `CRE_ETH_PRIVATE_KEY=YOUR_64_CHARACTER_PRIVATE_KEY_HERE`

open up `./src/workflows/hello-world/index.ts` to see the most basic cron-based example.

5. `cd` into `./src/workflows/hello-world` and then run `cre workflow simulate --target local-simulation --config config.json index.ts`
