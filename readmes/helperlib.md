This tooth package provides the interface type declaration file for the LLSE engine (in the format `.d.ts`)
## Usage
Running the following command will release the declaration file to the `declaration/llse/` folder in the command execution directory.
```shell
lip install helperlib
```
Add an `index.d.ts` to the head of the JS/TS script pointing to the `declaration/llse/` folder in the above command execution directory to introduce the declaration file.

If you are using git in the directory where the command is executed, it is recommended that you add `declaration/llse/` to `.gitignore`

### Get the HelperLib corresponding to the specified version of LL
Starting with LL 2.9.3 we add a Tag to each version of the complementary library for each LL release so that you can use Lip's version-specific installation feature to download the HelperLib for a specific LL version
