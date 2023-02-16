This tooth package provides the interface type declaration file for the LLSE engine (in the format `.d.ts`)
> This is a development dependency rather than a tool or LL plugin
## Usage
Running the following command to release the declaration file to the `declaration/llse/` folder in the command execution directory.
```shell
lip install helperlib
```
If your JS/TS code file is in the folder where you executed the above command add `/// <reference path=". /declaration/llse/index.d.ts" />` to introduce these declarations

### Get the HelperLib corresponding to the specified version of LL
Starting with LL 2.9.3 we add a Tag to each version of the complementary library for each LL release so that you can use Lip's version-specific installation feature to download the HelperLib for a specific LL version
