## Last updated 
28th March 2025

## Procedure followed

Here is the document/manual I followed to update the DB
https://github.com/tseemann/mlst?tab=readme-ov-file#updating-the-database 


Login to VIGASP-Galaxy VM. 
 
```
# Location of the DB
/opt/galaxy/21.09/database/dependencies/_conda/envs/__mlst@2.16.1/db

# Script to download
/opt/galaxy/21.09/database/dependencies/_conda/envs/__mlst@2.16.1/scripts

# Go into the scripts folder (you need to have write access!)
% cd /home/user/sw/mlst/scripts

# Run the downloader script (you need 'wget' installed)
% ./mlst-download_pub_mlst | bash

# Save the old database folder
% mv ../db/pubmlst ../db/pubmlst.old

# Put the new folder there
% mv ./pubmlst ../db/

# Regenerate the BLAST database
% ./mlst-make_blast_db

# Check schemes are installed
% ../bin/mlst --list
```

### Note:
```
# Here is the New DB
/opt/galaxy/21.09/database/dependencies/_conda/envs/__mlst@2.16.1/db/pubmlst
```
Updated DB contains two schemes for Ecoli (ecoli and ecoli_4)
Ecoli4 corresponds to Achtman 
Ecoli corresponds to Pasteur 




