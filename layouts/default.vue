<template>
  <div class="min-h-screen flex flex-col">
    <sys-omnibar>
      <template #global>
        <a
          href="https://system76.com/specials"
          target="_blank"
        >
          Special Offers
        </a>
      </template>

      <template #copy>
        <a
          href="https://system76.com/desktops"
          target="_blank"
        >
          New Thelio Accent Panels! Learn More!
        </a>
      </template>

      <template #local>
        <span :class="$style.hidden" />
      </template>
    </sys-omnibar>

    <sys-headerbar
      url-homepage="https://system76.com"
      url-laptops="https://system76.com/laptops"
      url-desktops="https://system76.com/desktops"
      url-mini="https://system76.com/desktops/meerkat"
      url-servers="https://system76.com/servers"
      url-keyboards="https://system76.com/accessories/launch"
      url-pop-os="https://pop.system76.com"
      url-contact="https://system76.com/contact"
      url-login="https://system76.com/login"
    />

    <nuxt class="flex-auto" />

    <sys-footerbar
      url-contact="https://system76.com/contact"
      url-about="https://system76.com/about"
      url-careers="https://system76.com/careers"
      url-specials="https://system76.com/specials"
      url-shipping="https://system76.com/shipping"
      url-financing="https://system76.com/financing"
      url-warranty="https://system76.com/warranty"
      url-privacy="https://system76.com/privacy"
      url-disclaimer="https://system76.com/disclaimer"
      url-terms="https://system76.com/terms"
    />
  </div>
</template>

<style>
html,
body,
#__nuxt,
#__layout {
  min-height: 100vh;
}
</style>

<style module>
/** This fixes an issue with the specials offers button hidden on tablet size **/
.hidden {
  display: none !important;
}
</style>
