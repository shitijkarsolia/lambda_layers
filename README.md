# Create an AWS Lambda Layer

#### 1. Create the project directory 
`mkdir project_dir`\
`cd project_dir`
#### 2. Create a Python3 Virtual Environment
`virtualenv -p /usr/bin/python3 venv`\
`source venv/bin/activate`
#### 3. Create the folder structure for the layer 
`mkdir -p lambda_layers/python/lib/python3.8/site-packages`
#### 4. Our current folder structure
```
├── project_dir
    └── lambda_layers
        └── python
            └── lib
                └── python3.8
                    └── site-packages
```
#### 5. Install the requred package using pip into the folder
`pip install xyz -t lambda_layers/python/lib/python3.8/site-packages/.`
#### 6. Change directory and zip
`cd lambda_layers`\
`zip -r xyz.zip *`
#### 7. Upload Zip in the Lambda Console



