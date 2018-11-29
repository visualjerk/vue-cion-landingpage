<template>
  <div>
    <ds-section
      primary
      id="usage">
      <ds-container width="large">
        <ds-heading tag="h2">Usage</ds-heading>
      </ds-container>
    </ds-section>
    <ds-section>
      <ds-container width="large">
        <ds-heading tag="h3">Integration in your application</ds-heading>
        <ds-text>It is recommended to integrate your design system as a private dependency via NPM. However, when first starting out, it is easier to keep it as a subfolder inside your application project.</ds-text>
        <ds-list ordered>
          <ds-list-item>
            <ds-space margin-bottom="x-small">Clone the design system to a subfolder of your project and install it's dependencies</ds-space>
            <ds-code>cd /path/to/your/project<br>git clone https://github.com/visualjerk/vue-cion-design-system.git design-system<br>cd design-system && yarn install</ds-code>
          </ds-list-item>
          <ds-list-item>
            <ds-space margin-bottom="x-small">Add it as a dependency to your project</ds-space>
            <ds-code>cd /path/to/your/project<br>yarn add file:./design-system</ds-code>
          </ds-list-item>
          <ds-list-item>
            <ds-space margin-bottom="x-small">Import and use it in your application entry (ex. main.js)</ds-space>
            <ds-code>import Vue from 'vue'<br><br>...<br><br>import DesignSystem from 'vue-cion-design-system'<br>import 'vue-cion-design-system/dist/system.css'<br>Vue.use(DesignSystem)<br><br>...</ds-code>
          </ds-list-item>
          <ds-list-item>
            <ds-space margin-bottom="x-small">Now you can use the design system's components in your application. Example:</ds-space>
            <ds-code>&lt;ds-button primary>Click me&lt;/ds-button></ds-code>
          </ds-list-item>
        </ds-list>
        <ds-heading tag="h3">Developing / Styleguide</ds-heading>
        <ds-text>When developing new or changing existing components, start the living styleguide to get direct feedback on your work. Also use the styleguide during development on your main project in order to find the components you need.</ds-text>
        <ds-code>cd /path/to/your/project/design-system<br>yarn dev</ds-code>
        <ds-heading tag="h3">Updating design system</ds-heading>
        <ds-text>The design system is added to your project as a npm dependency. Therefore you need to build it and update the dependency in order to see the changes in your actual project.</ds-text>
        <ds-list ordered>
          <ds-list-item>
            <ds-space margin-bottom="x-small">Build the system:</ds-space>
            <ds-code>cd /path/to/your/project/design-system<br>yarn build:lib</ds-code>
          </ds-list-item>
          <ds-list-item>
            <ds-space margin-bottom="x-small">Update the dependency:</ds-space>
            <ds-code>cd /path/to/your/project<br>yarn upgrade vue-cion-design-system</ds-code>
          </ds-list-item>
        </ds-list>
      </ds-container>
    </ds-section>
  </div>
</template>

<script>
export default {}
</script>
