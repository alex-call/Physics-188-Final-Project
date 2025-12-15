In order to save important output to a json, you must first create a .json file in this folder for it to be saved to.
This is unlike plots, for which a new file is created automatically when you run plt.savefig(...)

After the output variable(s) you wish to store are created, paste and modify the code snippet below based on your needs:

with open("output/output_data/your_file_name.json", 'w') as file:
    json.dump(
        {
            "Label1": var1,
            "Label2": var2,
            ...

        },
        file,
        indent=5
    )
