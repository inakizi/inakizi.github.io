---
title: <img src="/assets/img/fts/AppIcon_512_2x.png" width="100px" >&nbsp;&nbsp;False Tap Stop
filename: FalseTapStop
layout: page
subtitle: Prevent false taps when using "Tap to click" on your Mac
description: Fasle Tap Stop is a macOS app that prevents false taps when you have "Tap to click" configured in your Mac.
---


**False Tap Stop** Is a macOS application that prevents false taps when you have “Tap to click” configured in your Mac. It makes your Mac to ignore taps if they occur while keys are being pressed in the keyboard. The time to ignore taps after a key has been pressed is configurable in the application menu.

<img src="/assets/img/fts/mainscreen.png" >

<h3 id="faq">Frequently Asked Questions</h3>

#### How do I know the App is working?

With the time set to the default value of 500 milliseconds, rapidly type in a document while tapping the touchpad. The cursor should not jump to another location while tapping, and the number of “False Taps Stopped” in the application menu should increase every time you type.

#### What do I do if it is not working?

Open “System Preferences” and click on “Security & Privacy”. “False Tap Stop” needs “Accessibility” permissions to run. After making sure that “False Tap Stop” is checked, close the application and start it again. 

<img src="/assets/img/fts/accessibility2.png" >


#### I have a feature request, bug report, or some feedback

Please report it here:
<script defer src="https://js.statickit.com/statickit.js"></script>
<style type="text/css" media="screen">

.form-item {
   width: 100%;
}

.form-item label {
   display: block;
}

.form-item input {
   width: 100%;
}

.form-item textarea {
   width: 100%;
}


</style>


<form id="my-form">
   <div class="form-item">
   <label class="label" for="name">Name:</label>
   <input class="input is-medium" type="text" name="name">
   </div>

   <div class="form-item">
   <label for="email">Email:</label>
   <input id="email" type="email" name="email" value="" required />
   <div data-sk-error="email"></div>
   </div>

   <div class="form-item">
   <label class="label" for="message">Message:</label>
   <textarea class="textarea is-medium" placeholder="" name="message" minlength="20" rows="7" required></textarea>
   <div data-sk-error="message"></div>
   </div>

   <button type="submit">Submit</button>
</form>


<script>
  window.sk=window.sk||function(){(sk.q=sk.q||[]).push(arguments)};
  sk('form', 'init', {
    site: '7d12620bfabb',   // found under the Settings tab
    form: 'feedback',  // the key used in statickit.json
    element: '#my-form'       // a selector pointing to the `<form>` element
  });
</script>


<br>

#### Can you add support for macOS 10.13 or older?

No

#### Can you localize the app into my language?

I don't have any immediate plans to localize the app.
