A simple module for using [RRSSB](http://kurtnoble.com/labs/rrssb/) in Drupal.

It can be used like this:
```
  // Add RRSSB share buttons.
  $form['rrssb'] = array(
    '#markup' => srrssb(
      [
        'buttons' => ['googleplus', 'linkedin', 'facebook', 'twitter', 'email'],
        'url' => $url,
        'title' => $title,
        'summary' => $description,
        'hashtags' => $hashtags,
        'lng' => $lng,
      ]),
  );
```

It also provides this alter hook:
```
/**
 * Implements hook_srrssb_alter().
 * It is called by: drupal_alter('srrssb', $buttons, $options);
 */
function MODULE_srrssb_alter($buttons, $options) {

}
```
