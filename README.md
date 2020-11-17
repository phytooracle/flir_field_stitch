# Flir field stitch plot

Stitches corrected flir images into an orthomosaic.
 
## Inputs

Directory of all flir tif files.

## Outputs

Single stitched orthomosaic.

## Arguments and Flags
- **Required Arguments:** 
    - **Directory of flir files to stitch:** 'dir'
    - **Date of scan date:** 'scan_date' 

- **Optional Arguments**
    - **Output directory:** '-o', '--outdir', default='stitched_ortho_out/'
                                        
## Executing example (using singularity)
singularity run -B $(pwd):/mnt --pwd /mnt/ docker://phytooracle/flir_field_stitch -o <out_dir> -d <scan_date> <tif_dir>
