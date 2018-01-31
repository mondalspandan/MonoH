# Branch Reader

## Run on one sample

-- MonoHBranchReader.py can be used to run on a Skimmed Tree and it gives back one rootfile with signal region and control region histograms.

python MonoHBranchReader.py -a -i rootfilename -D . --csv

## Run on all samples

Use HTCondor and this repo: https://github.com/mondalspandan/bbDM-Tools/tree/master/BranchReader_HTCondor

# Skim Tree

## Run on one sample

-- SkimTree.py can be used to run on an ntuple and it gives back a smaller Skimmed Tree. SkimTree applies only very basic cuts.

python SkimTree.py ntuplerootfilename

## Run on all samples

Use HTCondor and this repo: https://github.com/mondalspandan/bbDM-Tools/tree/master/ST_BR_MultiParallel
(The ST_BR script runs both SkimTree and BranchReader steps in one go. It stores the SkimmedTrees in T2 and gives the BranchReader outputs as outputs of HTCondor).
