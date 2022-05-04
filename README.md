# Flask_backend

1. Clone the repository using "git clone https://github.com/PBL-Sem4/Flask_backend.git"
2. Set up the libraries by running
     pip install torch\
     pip install --upgrade tensorflow\
     pip install flax\
     pip install transformers\
     pip install sentencepiece\
     pip install flask\
     \
     Or simply run pip install -r /path/to/requirements.txt\
3. Run the main.py to start a local server
4. The test server will run on http://127.0.0.1:5000/ by default
5. Pass the text whose summary has to be found in the url bar after '/' (http://127.0.0.1:5000/Sample_text_whose_summary_has_to_be_found)
6. Since the code is compute heavy wait for 2-3 minutes for execution. For the first time it will take even longer as a 2.5GB model has to be downloaded.


