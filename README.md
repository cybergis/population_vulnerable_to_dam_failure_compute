# Populations Vulernable to Dam Failure CyberGIS-Compute Model

## Server-Side Work

1. Add the data mount to Keeling in `hpc.json`:

```
    "mount": {
      "/data/cigi/scratch/cigi-gisolve/compute_shared": "/compute_shared",
      "/data/cigi/common/jparkgeo/aging_dam_data": "/job/aging_dam_data"
    }
```

2. Add the SIF file to `container.json` (possibly add the mount here instead?):

```
  "extractinundationcensustracts-processor": {
    "dockerfile": "",
    "dockerhub": "",
    "hpc_path": {
      "keeling_community": "/data/keeling/a/cigi-gisolve/simages/extractinundationcensustracts-processor.sif"
  },
  "mount": {
  }
```