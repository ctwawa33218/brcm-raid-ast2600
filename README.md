# brcm-raid-ast2600

**Requirements:**

Get and install Git SPX Plugin (Preferrably link based building v1.0-beta7)
Get and install MDS-13.0

### v13-update-0.02 (06/19/2020) (It is alined with v13-update-0.02 release)

- Steps to apply featurepack

**US Location**
```
git clone --recurse-submodules https://git.ami.com/core/lts/spx-13/evb/ast2600evb.git --branch v13-update-0.02
cd ast2600evb/packages/
git clone --recurse-submodules https://git.ami.com/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git --branch v13-update-0.02-BRCM
```

**TW Location**
```
git clone --recurse-submodules https://git.ami.com.tw/core/lts/spx-13/evb/ast2600evb.git --branch v13-update-0.02
cd ast2600evb/packages/
git clone --recurse-submodules https://git.ami.com.tw/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git --branch v13-update-0.02-BRCM
```

**CN Location**
```
git clone --recurse-submodules https://git.ami.com.cn/core/lts/spx-13/evb/ast2600evb.git --branch v13-update-0.02
cd ast2600evb/packages/
git clone --recurse-submodules https://git.ami.com.cn/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git --branch v13-update-0.02-BRCM
```

*  [Link for fixed issues and change set]
(https://git.ami.com/groups/core/lts/spx-13/ext-packs/featurepack/brcm-raid/-/merge_requests?scope=all&utf8=%E2%9C%93&state=merged&milestone_title=v13-update-0.02-BRCM)

*  Please refer link https://git.ami.com/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600/-/wikis/ChangeLog for previous releases history


**Steps for compilation**

With 13.0 MDS

Below step converts packages to ".spx" format

git spx convert packages/ spx-packages/

* Open PRJ and spx-packages in MDS
* Update and save PRJ
* Please follow regular steps for source code compilation



### Active Tree Development:

**US Location**
```
git clone --recurse-submodules https://git.ami.com/core/lts/spx-13/evb/ast2600evb.git -b core_active_tree
cd ast2600evb/packages/
git clone --recurse-submodules https://git.ami.com/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git -b brcm-raid_active_tree
```
**TW Location**
```
git clone --recurse-submodules https://git.ami.com.tw/core/lts/spx-13/evb/ast2600evb.git -b core_active_tree 
cd ast2600evb/packages/
git clone --recurse-submodules https://git.ami.com.tw/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git -b brcm-raid_active_tree
```
**CN Location**
```
git clone --recurse-submodules https://git.ami.com.cn/core/lts/spx-13/evb/ast2600evb.git -b core_active_tree 
cd ast2600evb/packages/
git clone --recurse-submodules https://git.ami.com.cn/core/lts/spx-13/ext-packs/featurepack/brcm-raid/brcm-raid-ast2600.git -b brcm-raid_active_tree
```

**Steps for compilation**

With 13.0 MDS

Below step converts packages to ".spx" format

git spx convert packages/ spx-packages/

* Open PRJ and spx-packages in MDS
* Update and save PRJ
* Please follow regular steps for source code compilation