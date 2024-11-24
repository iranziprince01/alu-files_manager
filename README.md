# ALU Files Manager

ALU Files Manager is a robust, user-friendly file management system designed to streamline file organization and improve accessibility. Built with scalability and efficiency in mind, this project is ideal for students, faculty, and staff at the African Leadership University (ALU).

## Features

- **File Upload and Download**: Seamlessly upload files to the system and download them when needed.
- **Categorization**: Organize files by category, user, or specific tags for easy retrieval.
- **Search Functionality**: Advanced search options to quickly locate files based on keywords, file types, or categories.
- **User Access Control**: Role-based access ensures files are only accessible to authorized users.
- **Versioning**: Keep track of file changes with version control.
- **Cloud Storage Integration**: Supports integration with cloud services like Google Drive or Dropbox (optional).

## Technologies Used

- **Backend**: [Python] + [FastAPI]
- **Frontend**: [React.js] or [HTML/CSS/JavaScript]
- **Database**: [PostgreSQL] (or replace with your chosen database)
- **Authentication**: [OAuth2] or [JWT]
- **Cloud Storage**: [Amazon S3] (optional)
- **Containerization**: Docker for easy deployment and scalability.

## Installation

Follow these steps to set up the project locally:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/takurandoro/alu-files_manager.git
    cd alu-files_manager
    ```

2. **Set Up Virtual Environment**:
    ```bash
    python -m venv env
    source env/bin/activate   # On Windows use `env\Scripts\activate`
    ```

3. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Set Up Database**:
    - Install and set up PostgreSQL.
    - Create a database for the project and configure the `DATABASE_URL` in `.env`.

5. **Run Migrations**:
    ```bash
    alembic upgrade head
    ```

6. **Start the Application**:
    ```bash
    uvicorn app.main:app --reload
    ```

7. **Access the App**:
    Visit `http://127.0.0.1:8000` in your browser.

