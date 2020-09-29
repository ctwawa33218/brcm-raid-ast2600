# LTS-v13 BRCM-RAID-AST2600 (9/30/2020)

### Requirements

- Get and install **Git SPX Plugin** (Preferrably link based building v1.0-beta8)
- Get and install MDS-13

### Build Process
- Clone the project including submodules

    `<US Location>` :
    ```
    git clone --recurse-submodules https://git.ami.com/core/lts/spx-13/evb/ast2600evb.git --branch LTS-v13
    cd ast2600evb
    git submodule foreach git checkout LTS-v13
    cd packages 
    git clone --recurse-submodules https://git.ami.com/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git --branch LTS-v13
    cd brcm-raid-ast2600
    git submodule foreach git checkout LTS-v13
    ```
    `<TW Location>` :
    ```
    git clone --recurse-submodules https://git.ami.com.tw/core/lts/spx-13/evb/ast2600evb.git --branch LTS-v13
    cd ast2600evb
    git submodule foreach git checkout LTS-v13
    cd packages 
    git clone --recurse-submodules https://git.ami.com.tw/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git --branch LTS-v13
    cd brcm-raid-ast2600
    git submodule foreach git checkout LTS-v13
    ```
    `<CN Location>` :
    ```
    git clone --recurse-submodules https://git.ami.com.cn/core/lts/spx-13/evb/ast2600evb.git --branch LTS-v13
    cd ast2600evb
    git submodule foreach git checkout LTS-v13
    cd packages 
    git clone --recurse-submodules https://git.ami.com.cn/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git --branch LTS-v13
    cd brcm-raid-ast2600
    git submodule foreach git checkout LTS-v13
    ```
- Steps for compilation
    - With Git SPX Plugin 
    ```
    cd ast2600evb
    git spx buildsrc configs/ast2600evb.PRJ packages/ workspace_ast2600evb
    ```
    - With 13 MDS
        - Below step converts packages to ".spx" format
            ```
            git spx convert packages/ spx-packages/
            ```
        - Open `PRJ` and `spx-packages` in MDS
        - Update and save PRJ
        - Please follow regular steps for source code compilation



### Issues & Change Log
- [Link for list of fixed issues and its changeset after LTS-v13 release]( https://git.ami.com/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600/-/merge_requests?scope=all&utf8=%E2%9C%93&state=all&target_branch=lts-v13 )



