<template>
  <div>
    <ds-section 
      primary 
      id="first-steps">
      <ds-container width="large">
        <ds-heading tag="h2">First steps</ds-heading>
      </ds-container>
    </ds-section>
    <ds-section>
      <ds-container width="large">
        <ds-heading tag="h3">Setup</ds-heading>
        <ds-space>
          <ds-list
            ordered>
            <ds-list-item>
              <ds-space margin-bottom="x-small">
                Download the boilerplate
              </ds-space>
              <ds-code>git clone https://github.com/visualjerk/vue-cion-design-system.git your-system-name</ds-code>
            </ds-list-item>
            <ds-list-item>
              <ds-space margin-bottom="x-small">
                Install its dependencies
              </ds-space>
              <ds-code>cd your-system-name && yarn install</ds-code>
            </ds-list-item>
            <ds-list-item>
              <ds-space margin-bottom="x-small">
                Start development server
              </ds-space>
              <ds-code>yarn dev</ds-code>
            </ds-list-item>
          </ds-list>
        </ds-space>
        <ds-heading tag="h3">Design tokens</ds-heading>
        <ds-text size="large">Design tokens define the look and feel of your design system at the most basic level.</ds-text>
        <ds-text>To get a grasp of what design tokens are, open up <ds-code inline>src/system/tokens/font-size.yml</ds-code> in your editor.</ds-text>
        <ds-text>As you can see, every font-size value is represented by a meaningful name. Instead of hardcoding values in your codebase you can just refer to the name of each token.</ds-text>
        <ds-text>Your styleguide will automatically list these tokens in the section "Design Tokens":</ds-text>
        <ds-space margin-bottom="base">
          <img 
            src="../assets/font-size-design-tokens.png" 
            style="max-width: 100%">
        </ds-space>
        <ds-text>Now try updating the value for "font-size-body" to 17px and see how the styleguide adapts to your change.</ds-text>
        <ds-heading tag="h3">Adjusting colors</ds-heading>
        <ds-text>Open up <ds-code inline>src/system/tokens/color.yml</ds-code> in your editor.</ds-text>
        <ds-text>By default we use HSL to describe color tokens. This helps creating consistent colors throughout the application. If you don't know HSL yet, take a look at the <a
          href="http://hslpicker.com/" 
          target="_blank">HSL Color Picker</a>.</ds-text>
        <ds-heading tag="h4">Color hues</ds-heading>
        <ds-text>In order to keep the color token file DRY, base hues are listed under "aliases". Each alias stands for hue + saturation. Try to adjust the value for "teal" and see how that affects the styleguide.</ds-text>
        <ds-heading tag="h4">Color tokens</ds-heading>
        <ds-text>The actual color tokens are listed under "props". Try changing the "color-primary" and its variations to use blue instead of teal and see the effect on the styleguide.</ds-text>
        <ds-heading tag="h3">Creating your design</ds-heading>
        <ds-space
          margin-top="base"
          margin-bottom="base">
          <img 
            src="../assets/customize-design-tokens.png" 
            style="max-width: 100%">
        </ds-space>
        <ds-text>Have a look at the examples inside <ds-code inline>src/system/tokens/_examples</ds-code> to get an idea of what is possible. You can try to overwrite the tokens in the main folder with those in the examples subfolders.</ds-text>
        <ds-text>Now you can start to create your own design by adjusting the design tokens to your taste. <ds-text bold>Enjoy!</ds-text></ds-text>
      </ds-container>
    </ds-section>
  </div>
</template>

<script>
export default {}
</script>
