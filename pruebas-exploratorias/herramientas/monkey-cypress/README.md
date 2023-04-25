# Cypress Random Tester (Monkey) for Ghost
1. Start Ghost server on port 2368
2. Go to http://127.0.0.1:2368/ghost/
3. Create a user with email `monkey@example.org` and password `0123456789!`
4. Install dependencies with `npm install`
5. Run tests with monkey with `docker run --rm -it -v $PWD:/e2e -w /e2e --add-host host.docker.internal:host-gateway cypress/included:4.11.0 -C monkey-config.json`
6. Run tests with smart-monkey with `docker run --rm -it -v $PWD:/e2e -w /e2e --add-host host.docker.internal:host-gateway cypress/included:4.11.0 -C smart-monkey-config.json`
