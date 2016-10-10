# ui_component
Implementation of ui component convention in coffescript

Usage
```
class HeaderComponent extends wunderLib.UIComponent

  _initUI: ->
    @$openMenuTrigger = @$container.find('.js-menu-trigger')
    @$menu = @$container.find('.js-menu')

  _initEventListeners: ->
    @$openMenuTrigger.on 'click', (e) =>
      @openMenu()

  openMenu: ->
    @$openMenuTrigger.toggleClass('open')
    @$menu.toggleClass('open')

```
