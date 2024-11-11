## Wallpaper Application Backend

This is the backend of the wallpaper application. It is a [Directus](https://directus.io/) project that uses SQLite as the database.

Frontend: [Wallpaper Application Frontend](https://github.com/CallSignRishav/wallpaper-frontend)

## Getting Started

If you want to run this project, you need to follow the steps below:

1. Create a `.env` file in the root directory of the project and copy all the code from `.env.example` and paste it into `.env` file.

2. Install the dependencies:

```bash
npm install
```

3. Bootstrap the database:

```bash
npm run bootstrap
```

4. Migrate the database schema:

```bash
npm run apply
```

5. Start the server:

```bash
npm start
```

## Important Notes

If you manually upgrade the Directus version, don't forget to migrate the database schema:

1. Take a snapshot of the database.

```bash
npm run snapshot
```

2. Apply the snapshot to the new Directus version.

```bash
npm run apply
```

3. Migrate the database schema.

```bash
npm run migrate
```
