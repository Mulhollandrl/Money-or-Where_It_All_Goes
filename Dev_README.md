# Dev README

This is a guide to get you up and ready to contribute to this application! You need to complete **ALL** parts of this guide before developing, or things will break.

## NEVER DEVELOP ON THE MAIN BRANCH

## Table of Contents:

- **[Necessary Installations](#necessary-installations)**

- **[Setting Up The Backend](#setting-up-the-backend)**

- **[Setting Up The Frontend](#setting-up-the-frontend)**

- **[Setting Up Docker](#setting-up-docker)**

- **[References](#references)**

## Necessary Installations:

You will need a few things pre installed to develop on this project:

- Python 3.12.0
- Node.js 20.11.0
- Docker Desktop
- Docker Compose
- You can install the rest in the next steps

## Setting Up The Backend:

I suggest using a python virtual environment for this, but it is not required. You **NEED** to make sure you are using the versions listed in the last step though. I would also suggest using two separate terminals for these next two steps.

In your terminal, navigate to the backend directory:
```bash
cd backend
```

You will now install all of the requirements:
```bash
pip install -r requirements.txt
```

Then you will run the [manage.py](backend/manage.py) script:
```bash
python manage.py runserver
```

## Setting Up The Frontend:

I would recommend doing this in a separate terminal from the last step.

You will first navigate to the frontend folder:
```bash
cd frontend
```

Then you will install all of the necessary node_modules:
```bash
npm install
```

You can then start the frontend:
```bash
npm start
```

## Setting Up Docker:

Now we will set up the containers using Docker. This helps us all keep VERY similar development environments, and cuts down on us having versioning issues.

First, you want to navigate to the root directory of this project (likely something like "/Money/"). I would also recommend doing this part in a separate terminal window from the last two steps:
```bash
cd Money
```

After that, you will need to build the container itself. You can do this by building with docker compose:
```bash
docker-compose build
```

You then want to start the container. You can do this by running:
```bash
docker-compose up
```

You can stop the containers in one of three ways. You can go to the Docker Desktop app and stop them with the GUI, you can use ```ctrl+c``` in the place you started them, or you can run:
```bash
docker-compose down
```

### You should now be fully set up and ready to develop! If you go to ```localhost:3000``` to see the results.

## References:

https://dev.to/anjalbam/dockerize-a-django-react-and-postgres-application-with-docker-and-docker-compose-by-anjal-bam-e0a