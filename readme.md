**Look for more information in the documentation

Obs.: start git before 

Tools used:
 - commitlint:
    npm i -D @commitlint/config-conventional @commitlint/cli
    echo "module.exports = {extends: ['@commitlint/config-conventional']}" > commitlint.config.js

 - husky:
    npm i -D husky
    npx husky install
    npx husky add .husky/commit-msg  'npx --no -- commitlint --edit ${1}'


convention: 
    type(scope?): subject

Example of convention:
    chore: run tests on travis ci
    fix(server): send cors headers
    feat(blog): add comment section

Types of modification:
    build
    chore
    ci
    docs
    feat
    fix
    perf
    refactor
    revert
    style
    test


****