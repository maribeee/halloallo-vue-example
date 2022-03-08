#Alex check out these pages:

* `src/App.vue` for the primary app page, this is where the event component is initiated, also you can see the list of events that is passed to the Event component in the data object in the `<script>` tag. It's a JSON object that in a live version of this site would be pulled from the database

* `src/components/Event.vue` you can see that it is a single instance of the event component that iterates through every event in the JSON events object. This way you don't have to create a new event component for each event, it just automatically makes them for you! You only need to make one and it creates one for each event in the events object.

This can also be done for example for the categories and all your inputs etc, and you could create functions that can sort the events by name or by date or something very easily etc etc

Let me know if you have questions


#hallo-vue-example

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=johnsoncodehk.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=johnsoncodehk.vscode-typescript-vue-plugin).

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```
