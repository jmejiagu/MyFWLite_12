# MyFWLite CMSSW_12_0_2

## Intructions to run the examples.
```
source /cvmfs/cms.cern.ch/cmsset_default.sh
export SCRAM_ARCH=slc7_amd64_gcc900
cmsrel  CMSSW_12_0_2
cd CMSSW_12_0_2/src/
cmsenv
voms-proxy-init -voms cms -valid 192:00
git clone git@github.com:jmejiagu/MyFWLite_12.git DataFormats/FWLite
scram b
```

Run: (use your favorite MiniAOD input sample. You will see J/psi and Zmass peak examples)

```
python3 DataFormats/FWLite/examples/bin/Jpsi_peak.py inputFiles=/eos/cms/store/relval/CMSSW_12_1_0_pre2/RelValPsi2SToJPsiPiPi_14/MINIAODSIM/121X_mcRun3_2021_realistic_v1-v3/10000/934b45ff-3f99-4f69-9648-bfd129ab7d90.root
```


