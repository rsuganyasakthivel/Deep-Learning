Step 1: Inside frontend folder open gitbash. Use the following commands.
  npm intall --from-lock-json
  npm audit fix

  
Step 2: Create .env file having the url of your FastAPI server. 


Step 3: give the following command in gitbash(in frontend directory)
  npm run start

  
Step 4. run the backend server. main.py OR main-tf-serving.py
  If tf-serving to be used, before running backend server,
  
    i. open docker desktop
    
    ii. run the following cmd on window powershell:
      docker run -t --rm -p 8502:8502 -v D:/DeepLearning/CNN/Mango_Leaf_Disease_Classification:/Mango_Leaf_Disease_Classification tensorflow/serving --rest_api_port=8502 --model_config_file=/Mango_Leaf_Disease_Classification/models.config

      
Step 5: Drag an image of a mango leaf in the website. You would see the prediction.
  
