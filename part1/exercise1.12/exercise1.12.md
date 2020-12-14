# Solution to exercise 1.12

- commands used:
    - docker build -t frontend-example .
    - docker build -t backend-example .

    - docker run -d --rm -p 5000:5000 frontend-example
    - docker run -d --rm -p 8000:8000 backend-example
