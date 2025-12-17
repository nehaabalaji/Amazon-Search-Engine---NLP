## How to run the code 

To execute the full project successfully and ensure the retrieval pipeline runs fast, follow these steps:

1. Convert the dataset to CSV  
   The original file may be named reviews_segments.xlsx  
   Open it on your computer and export or save it as reviews_segment.csv.  
   The project is written to read a CSV file, so using an XLSX file will not work.  
   
2. Upload the CSV into Google Colab  
   Open the notebook (NLP_Project_FINAL.ipynb) in Google Colab.  
   In the left sidebar, open the Files tab and upload your reviews_segment.csv manually.  
   The file must appear in the /content/ directory for the code to run correctly.  
   
3. Change the runtime settings  
   Go to the top menu → Runtime → Change runtime type.  
   Set the hardware accelerator to GPU.  
   If available, select the A100 GPU option for the fastest execution. This is what I used with Google Colab Pro 
   This helps reduce time for preprocessing, TF-IDF vectorization, and ML operations.  
   
4. Ensure libraries and dependencies  
   All required libraries and dependencies are already included and imported in the first cell of the notebook.  
   You do not need to manually install anything.  
   Simply run the notebook cells in order.  
   
5. Run all cells at once  
   After uploading the dataset and setting the runtime, click Runtime → Run all.  
   The notebook will automatically perform the following steps:  
    load the dataset  
    preprocess the review text  
    run Baseline retrieval  
    run Method 1, Method 2, Method 3, and Method 4  
    execute all test queries  
    print method-specific outputs under each section  
    build and display the final precision comparison table  
    
6. Output files  
   Any generated files or tables will appear in the Colab file area.  
   You can download these files directly if you need to include them in your submission or documentation.  
   
7. Expected execution time  
   With an A100 GPU, the entire pipeline (from preprocessing through all retrieval methods and final evaluation) typically finishes in 10 to 15 minutes, even with the full 210,000-review dataset.  
   Using CPU-only mode may take way longer.  
   
8. Verify results  
   Scroll through the notebook to confirm that:  
    every method prints its outputs for each test query  
   saved files appear in the file area  
   the last section displays the complete precision evaluation table  
   


