# Flask_backend

1. Clone the repository using "git clone https://github.com/PBL-Sem4/Flask_backend.git"
2. Set up the libraries by running
     pip install torch
     pip install --upgrade tensorflow
     verify tf install by running python -c "import tensorflow as tf;print(tf.reduce_sum(tf.random.normal([1000, 1000])))"
     pip install flax
     pip install transformers
     pip install sentencepiece
     pip install flask
3. Run the main.py to start a local server
4. The test server will run on http://127.0.0.1:5000/ by default
5. Pass the text whose summary has to be found in the url bar after '/' (http://127.0.0.1:5000/<text whose summary you want>)
6. Since the code is compute heavy wait for 2-3 minutes for execution. For the first time it will take even longer as a 2.5GB model has to be downloaded.


