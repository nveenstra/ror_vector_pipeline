# ror_vector_pipeline
Build vectors for ror organizations and store in postgres database

## goal

Create ROR vectors in order to match with external organizations in the Pure research information system. Vector generation is working: steps to execute:

- Clone project locally
- Install postgres 
- Create database, e.g. ror_db
- Update database connection settings in the notebook accordingly
- Download latest ror dump from here: https://zenodo.org/records/17468391
- Put downloaded zip file in project folder next to the notebook file
- Rename zip to 'ror-latest.zip'

Then run the notebook cells one by one. Use cell 0 to delete existing tables and start over. Step 1 installs the multilingual‑e5‑large model used for the embeddings. Make sure you have enough (GPU) memory to run the model; this notebook was developed on a mac with unified memory.
After cell 6 check if all tables are filled correctly before proceeding. 

This notebook will be updated with Pure external organization logic.
