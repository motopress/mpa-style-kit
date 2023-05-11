<p align="center">
  <a href="https://motopress.com/products/appointment-booking/">
    <img src="https://ps.w.org/motopress-appointment-lite/assets/icon.svg" width="128" height="128" alt="MotoPress Appointment Booking">
  </a>
</p>

<h2 align="center">MotoPress Appointment Booking Style Kit</h2>

This boilerplate is designed for WordPress theme developers who are interested in developing themes with the MotoPress Appointment Booking plugin.

This Style Kit provides smartly organized starter scss files to style [**MotoPress Appointment Booking**](https://motopress.com/products/appointment-booking/).

The MotoPress Appointment Booking plugin makes it easy for businesses to accept bookings and appointments online. It’s geared to time and service-based companies, such as for beauty, sports, education, and other industries. Staff planning, real-time bookings of any custom time slots, and timely appointment schedules at your fingertips.

See also: [Pre-made Appointment Booking Themes](https://motopress.com/products/category/appointment-wordpress-themes/)

## For themes built using SASS/SCSS

1. Download a zip folder/clone a repository.
2. Copy the `scss` directory and paste it to the sass/scss directory of the theme styles.
3. Import `style.scss` at the end of the main file containing styles.
4. Have fun!

## For themes built without SASS/SCSS

1. Download a zip folder/clone a repository.
2. Run a console command `npm i`.
3. Run a console command `npm run watch` (this will run a task that will watch for changes in .scss files).
4. Add generated `style.css` to your theme.
5. Have fun!

## Useful theme support snippets

### Enqueuing the style to your theme

Add the following snippet into `functions.php`:

```
wp_enqueue_style( 'mpa-style-kit', 'path_to_compiled_style/style.css', array(), '1.0.0' );
```

### Enqueuing the style to Block Editor

If you are using default Block Editor, and want load styles there - then add the following snippet into `functions.php`:

```
add_theme_support('editor-styles');

add_editor_style( array(
    'path_to_compiled_style/style.css',
    /* here can be url to Google Font, or another style file */
) );
```

## Directory structure
For your convenience, all styles are logically divided into files. All files contain templates with the minimum set of selectors for styling different blocks.

```
mpa-style-kit
├───css                       # compiled css will be here
└───scss
    ├───abstracts             # some helpers
    │   └───_grid.scss
    ├───shortcodes            # shortcode-related styles
    │   ├───employee
    │   │   ├───_additional-info.scss
    │   │   ├─── ...
    │   │   └───_title.scss
    │   ├───_appointment-form.scss
    │   ├─── ...
    │   └───_services-list.scss
    ├───widgets               # widget-related styles
    │   └───_appointment-form.scss
    ├───_employee-attributes.scss
    ├─── ...
    ├─── _single-service.scss
    └───style.scss            # main style file
```

## License
MotoPress Appointment Booking Style Kit, Copyright &copy; 2023, MotoPress. MotoPress Appointment Booking Style Kit is distributed under the terms of the [GPLv2](http://www.gnu.org/licenses/gpl-2.0.html).

<p align="center">
    <br/>
    Made with 💙 by <a href="https://motopress.com/">MotoPress</a>.<br/>
</p>