# LTS-v13 BRCM-RAID-AST2600 (9/30/2020)

### Important Information
- After Stable release features migrated into the active branch ("LTS-v13"), the tag "v13-update-X.XX-RC"  is created in each repository. The tag is just providing the information "when the milestone New feature/feature enhancement migration Finished" Only.**_ The latest Active branch always provides the latest Bug fixed and Feature enhancement. Please take the latest Active Branch for the project development.

### Requirements

- Get and install the released **Git SPX Plugin v1.0-beta9.3.2** version
- Get and install the latest released MDS version

### Build Process
- Clone the project including submodules

    `<US Location>` :
    ```
    git clone --recurse-submodules https://git.ami.com/core/lts/spx-13/evb/ast2600evb.git --branch LTS-v13
    cd ast2600evb/packages
    git clone --recurse-submodules https://git.ami.com/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git --branch LTS-v13
    cd brcm-raid-ast2600
    git submodule foreach git checkout LTS-v13
    git checkout LTS-v13
    git pull origin LTS-v13
    cd ../..
    git submodule foreach git checkout LTS-v13
    git checkout LTS-v13
    git pull origin LTS-v13
    ```
    `<TW Location>` :
    ```
    git clone --recurse-submodules https://git.ami.com.tw/core/lts/spx-13/evb/ast2600evb.git --branch LTS-v13
    cd ast2600evb/packages
    git clone --recurse-submodules https://git.ami.com.tw/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git --branch LTS-v13
    cd brcm-raid-ast2600
    git submodule foreach git checkout LTS-v13
    git checkout LTS-v13
    git pull origin LTS-v13
    cd ../..
    git submodule foreach git checkout LTS-v13
    git checkout LTS-v13
    git pull origin LTS-v13
    ```
    `<CN Location>` :
    ```
    git clone --recurse-submodules https://git.ami.com.cn/core/lts/spx-13/evb/ast2600evb.git --branch LTS-v13
    cd ast2600evb/packages
    git clone --recurse-submodules https://git.ami.com.cn/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git --branch LTS-v13
    cd brcm-raid-ast2600
    git submodule foreach git checkout LTS-v13
    git checkout LTS-v13
    git pull origin LTS-v13
    cd ../..
    git submodule foreach git checkout LTS-v13
    git checkout LTS-v13
    git pull origin LTS-v13
    ```
- Steps for compilation
    - With Git SPX Plugin 
        ```    
        cd ast2600evb    
        git spx buildsrc configs/ast2600evb_A1.PRJ packages/ workspace_ast2600evb
        ```
    - With MDS (latest released version)
        - Below step converts packages to ".spx" format
            ```
            git spx convert packages/ spx-packages/
            ```
        - Open `PRJ` and `spx-packages` in MDS
        - Update and save PRJ
        - Please follow regular steps for source code compilation



### Issues & Change Log
- [Link for list of fixed issues and its changeset after LTS-v13 release]( https://git.ami.com/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600/-/merge_requests?scope=all&utf8=%E2%9C%93&state=all&target_branch=LTS-v13 )



