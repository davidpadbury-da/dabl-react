# @daml/dabl-react

> React functions for DAML applications running on [projectDABL](https://projectdabl.com/).

## Documentation

This library aims to complement [@daml/react](`https://www.npmjs.com/package/@daml/react),
to make it easier to write [React](https://reactjs.org/) applications on DABL specifically.
To that end we provide for convenience.

## Usage

### Well Known End point

DABL provides an `.well-known` endpoint ([see](https://docs.projectdabl.com/api/onboarding/#listening-for-new-users)), that provides the identity of Party's who can run automation or
observe common information for your application.

```typescript
// Within a
<WellKnownPartiesProvider>
  ...
  // This hook will this object from DABL.
  let wkp : WellKnownParites = useWellKnownParties();

</WellKnownPartiesProvider>
```

### Information within the JWT.

```typescript
let usersPartyName = partyName(token);
let needToResetLogin = expiredToken(token);
```

## Source
TODO

## License
TODO