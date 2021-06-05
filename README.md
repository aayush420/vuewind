## Vuewind - Just another component library using Vue & Tailwindcss

### Installation
1. The npm package can be installed using `npm i @aayush420/vuewind` or `yarn add @aayush420/vuewind` if you are using yarn.
2. Once the package is installed, the components and styles are to be imported. 
    - The components can be imported into individual components like this -
    `import { VButton } from '@aayush420/vuewind'`
    - The styles can be imported globally in your index.css like this - 
    `@import '../node_modules/@aayush420/vuewind/dist/style.css'`

### Usage
Once the components are imported, tey can directly be invoked inside your components like this -
`<VButton v-text="'Hello123'" @click="some_func" class="extra-classes-if-needed" />`
