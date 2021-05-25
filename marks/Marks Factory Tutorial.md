# Marks Factory Tutorial

## Intro

This is the Marks Factory.

### Top Toolbar
:Button[more]{icon=true} load a recommended mark
:Button[play]{icon=true}  enter "play" mode. This is how your mark is presented to the user.
:Button[edit]{icon=true}  enter "edit" mode.
:Button[export]{icon=true} export your mark to IPFS. If your mark uses contract ABIs and addresses from your workspace, they will also be exported. You will see a QRcode image and if you click on it, the URL will be copied to the clipboard. The URL is of the form `<BASE_URL>/?ipfs=<IPFS_HASH>&input=<PREDEFINED_INPUT>`. You can preset form inputs by filling them in and then exporting.
:Button[eth]{icon=true} Load a contract function form, from the ABIs and addresses saved in the workspace
:Button[bold]{icon=true} - :Button[deindent]{icon=true} markdown syntax helpers

### Bottom Workspace

Add contract ABI & address information by:
- clicking on the bottom left :Button[more]{icon=true} -> Add item -> filling the form; if you fill in an IPFS hash from a contract saved in the Solidity compiler format, the abi will be loaded automatically -> click on the bottom right :Button[^]{}
- pasting JSON data in the bottom text area, of the form:
```
[{
    "ipfs": "QmP5rC8m7DsZwmRjFr7PESKe9e9o7p7VVNP62jdBbiCGbQ",
    "name": "WETH",
    "address": "0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
    "abi": []
}]
```

## Add your mark to the menu recommendations

Make a Pull Request to https://github.com/loredanacirstea/recommendations/blob/main/marks/mainMenu.json and add your mark under an existing category or propose a new category.

### Requirements
- title of the form: `<TITLE> v<VERSION>`, e.g. `Mark Title v1`
- mark contains a video tutorial of how to use the mark
- add a :Link[created by 0x<ETH_ADDRESS>]{} at the bottom of your mark
- the mark's "label" is the same as its title
- export your mark to IPFS first and use the 46 character hash as the mark's value id (e.g. `QmadhiGumnFNeHf8pJge6A2sdunVNXH6VnLuFFvzsAbieC`)

### Info
- if your mark has been approved, updating the mark to a new version will be prioritized
- if a similar mark already exists, make a PR only if your mark brings significant improvements.

### Resources

- Marks Factory playlist https://www.youtube.com/playlist?list=PL323JufuD9JBUwKSPILGKBaI5JPyAVapn


