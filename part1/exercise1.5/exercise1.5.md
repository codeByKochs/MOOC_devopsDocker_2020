# Solution to exercise 1.5

- commands used:
    - docker run --name ubuntu --rm ubuntu:16:04
    - docker exec -ti ubuntu sh -c "echo 'Input website:'; read website; echo 'Searching...'; sleep 1; curl http://www.$website;"
    - helsinki.fi