# NodeJS

## Avoid object truncated when using console.log()

```javascript
console.dir(obj, { depth: Infinity });
```

## use project as a local library
Modify your library.

To use the newly modified project localy:
- Update the library version in package.json on both the project using the library and the library itself.

## Test
```bash
# in library repository
# no need to change version for now
npm run build # necessary in Typescript, optionnal in javascript
npm link

# in project using the library
sudo npm link @callbot/cb-common
```
/!\ Do not commit the version change in the library repository! It will be handled in the publish part below.

## Publish
Once the project is ready, publish the library
```bash
# Change version 

npm version minor
# → Incrémente la version mineure (1.8.x → 1.9.0)
npm version patch
# → Incrémente uniquement le patch (1.8.1 → 1.8.2)
npm version major
# → Incrémente la version majeure (1.x.x → 2.0.0)
npm version <version>
# → Définit une version exacte

git push --no-verify
git push --tags --no-verify


npm publish
```
