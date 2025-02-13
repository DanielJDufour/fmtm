<svelte:head>
  <script src="https://danieljdufour.com/web-forms-web-component/odk-web-form.js" type="module"></script>
</svelte:head>

<script>
  import { page } from '$app/stores';
  console.log("in frame page is:", page);

  console.log("parent is:", window.parent);

  // : Props = $props();
  // import { expose } from 'microlink';

  // console.log("expose:", expose);
  // // install microlink and expose following functions:
  // // reset, save

  // const reset = ({ formXml }) => {
  //   console.log("resetting form with xml", formXml);
  // };

  // expose({
  //   reset
  // });
</script>

<div style="height: 500px; overflow-y: scroll">
  <odk-web-form form-xml="https://danieljdufour.com/web-forms-web-component/whova_form-BvHYggiJ.xml"></odk-web-form>
</div>

