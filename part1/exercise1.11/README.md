# Solution to exercise 1.11

- commands used:
    - docker build -t exercise1.11 .
    - docker run -d -p 8000:8000 --name exercise1.11 --rm -v $(pwd)/logs.txt:/logs.txt exercise1.11
