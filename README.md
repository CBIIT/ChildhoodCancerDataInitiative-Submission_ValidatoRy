# ChildhoodCancerDataInitiative-Submission_ValidatoRy
This script will take a CCDI metadata manifest file and validates the submission based on the model found in the template file. This is based on the CCDI-Submission_ValidatoR.R script.

This is a refactoring of the [CCDI-Submission_ValidatoR](https://github.com/CBIIT/ChildhoodCancerDataInitiative-Submission_ValidatoR/tree/main) code into python.

This python script takes a data file that is formatted to the [submission template for CCDI](https://github.com/CBIIT/ccdi-model/tree/main/metadata-manifest) as input. It will output a file that describes whether sections of the Metadata table PASS, ERROR or WARNING on the checks.

To run the script on a CCDI template, run the following command in a terminal where python3 is installed for help.

```
python CCDI-Submission_ValidatoRy.py -h
```

```
usage: CCDI-CatchERRy.py [-h] -f FILENAME -t TEMPLATE [-p S3_PROFILE]

This script will take a CCDI metadata manifest file and validates the submission based on the model found in the template file. This is based on the CCDI-
SubmissionValidationR.R script.

optional arguments:
  -h, --help            show this help message and exit
  -f FILENAME, --filename FILENAME
                        dataset file (.xlsx, .tsv, .csv)
  -t TEMPLATE, --template TEMPLATE
                        dataset template file, CCDI_submission_metadata_template.xlsx
  -p S3_PROFILE, --s3_profile S3_PROFILE
                        The s3 bucket profile associated with the access to the s3 bucket.
```
