# How to use - Method 2
In this method you initialise your new CRE project with `cre-init`. If there is no package.json in your

# How to use - Method 2

In this method you use existing TS workflows in the `src/workflows` directory __without__ first running `cre init`.

TODO -- bun (https://bun.com/) && "postinstall": "bunx cre-setup"

1. Git clone the CRE CLI into a different directory and run the build command specified in the CLI's README so that you have the `cre` executable in that project's root. For me the `cre` cli executable is in `"/Users/zubinpratap/code/cre-cli/`

2. `bun install` to install the dependencies of this examples project. Then run `bunx cre-setup` to setup the CRE TS SDK. You should see `✅ CRE TS SDK is ready to use.` in the terminal.  

3. alias `cre to` point to the cre executable that you built previously. For me it looks like
   `alias cre="/Users/zubinpratap/code/cre-cli/cre"`

4. set copy `.env.example` into a `.env` file with `CRE_ETH_PRIVATE_KEY=YOUR_64_CHARACTER_PRIVATE_KEY_HERE`

open up `./src/workflows/hello-world/index.ts` to see the most basic cron-based example.

5. `cd` into `./src/workflows/hello-world` and then run `cre workflow simulate --target local-simulation --config config.json index.ts`
