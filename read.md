Lets setup a project for Bootstrap 5 Alpha
Setup the same workflow with npm do need 

- npm init -y
- npm i bootstrap@next OR
- npm i bootstrap@5.0.0-alpha1
- npm i bootstrap-icons (all the svg icon )

- install Sass compiler 
- go to the setting cmd+shift+p
- open setting
- type live sass -> click on edit json in
Live Sass Compile › Settings: Formats
Set your exported CSS Styles, Formats & save location.
- create a folder scss -> and file main.scss

how to use utility API
node_modules->bootstrap->scss->utilities.scss

// Utilities
$utilities: ()!default;
$utilities: map-merge(
        (
            'input-padding': (
            property: padding,
            class: ip,
            values:(
                0: 0,
                1: 0.3rem,
                2: 0.5rem,
                3: 0.7rem,
                4: 0.9rem,
                5: 1rem,
            ),
        ),
    ),
    $utilities
);

- To include JS you can use CDN, V5 GetBootstrap.com or from the node modules
<script src="/node_modules/bootstrap/dist/js/bootstrap.min.js"></script>
- you might need pooper.js
<script src="/node_modules/popper.js/dist/popper.min.js"></script>