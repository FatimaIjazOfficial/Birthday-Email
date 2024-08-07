# Birthday Email 

The Birthday Email  is designed to automatically send personalized birthday emails to recipients on their special day. The program reads birthday data from a CSV file and uses pre-written letter templates to create customized birthday messages.

## Description

This program performs the following tasks:

1. Reads birthday data from a CSV file (`birthdays.csv`).
2. Checks if today's date matches any birthday in the CSV file.
3. Selects a random letter template from the `letter_templates` directory.
4. Sends a personalized birthday email to the recipient using the selected template.

## Usage Instructions

### 1. Setup Email Password

To use this program, you need to create an App Password for your email account. Follow these steps:

- Go to [Google Account](https://myaccount.google.com/).
- Select **Security** on the left and scroll down to **How you sign in to Google**.
- Find the section on **App Passwords** by searching for it.
- Create an App Password for your email (e.g., Python Mail) and click create.
- Copy the generated 16-character password. This is the only time you will see the password.

### 2. Configure Email Credentials

Update the `email` and `password` variables in the `main.py` script with your email address and the generated app password.

### 3. Prepare Birthday Data

Create a `birthdays.csv` file with the following structure:

```csv
name,email,year,month,day
example_name,example@example.com,1990,7,6
```

- `name`: Name of the birthday person.
- `email`: Email address of the birthday person.
- `year`: Birth year of the birthday person.
- `month`: Birth month of the birthday person.
- `day`: Birth day of the birthday person.

### 4. Create Letter Templates

Create a directory named `letter_templates` and add your letter templates as text files (`letter_1.txt`, `letter_2.txt`, `letter_3.txt`, etc.). Each template should include `[NAME]` as a placeholder for the recipient's name. Example:

```text
Dear [NAME],

Happy birthday!

All the best for the year!

Your Name
```

### 5. Run the Program

Run the `main.py` script. The script will:

- Read the birthday data from `birthdays.csv`.
- Check if today's date matches any birthday.
- Select a random letter template from the `letter_templates` directory.
- Send a personalized birthday email to the recipient using the selected template.

### Requirements

- Python 3.x
- `pandas` library (install using `pip install pandas`)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

This README provides a clear description of the program and detailed usage instructions, including setting up email credentials, preparing birthday data, creating letter templates, and running the program. Let me know if you need any further adjustments or additions!
