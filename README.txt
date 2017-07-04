cd /Users/raynovarina/Sites/AtomProjects/harp/photo-effects

Created and initialized harp app:

$ /Users/raynovarina/Sites/AtomProjects

$ harp init photo-effects

$ cd photo-effects

Change main.less to:
/* empty */

Change index.jade:
  h1 Welcome to harp/photo-effects.
  h3 Deployed locally at http://localhost:9000/
  h3 Deployed on Heroku at https://harp-photo-effects-94037.herokuapp.com/

Add package.json and Procfile files for Heroku deploy:
  package.json:

    {
      "name": "harp-heroku-photo-effects",
      "version": "1.0.0",
      "description": "A Harp App on Heroku",
      "dependencies": {
        "harp": "*"
      }
    }

  Procfile:

    web: harp server --port $PORT

At github account, create new repository: harp-heroku-photo-effects and then
locally.
  $ git init
  $ git remote add origin https://github.com/RayNovarina/harp-heroku-photo-effects.git

Create Heroku app:
  $ heroku create harp-photo-effects-94037

$ git remote -v
  heroku  https://git.heroku.com/harp-photo-effects-94037.git (fetch)
  heroku  https://git.heroku.com/harp-photo-effects-94037.git (push)
  origin  https://github.com/RayNovarina/harp-heroku-photo-effects.git (fetch)
  origin  https://github.com/RayNovarina/harp-heroku-photo-effects.git (push)

Deploy changes to github and heroku:
  $ git add .
  $ git commit -am "First Harp + Heroku commit"
  $ git push origin master
  $ git push heroku master

View on Heroku:

  https://harp-photo-effects-94037.herokuapp.com shows:

  Welcome to harp/photo-effects.
  Deployed locally at http://localhost:9000/
  Deployed on Heroku at https://harp-photo-effects-94037.herokuapp.com/

===============================
<!DOCTYPE html>
<html lang="en">

<head>
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="description" content="Sandbox for harp-heroku trr-photo-effects" />
<!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
<title>harp-heroku trr-photo-effects</title>

<link rel="stylesheet/less" type="text/css" href="//localhost:9000/Sites/AtomProjects/harp/photo-effects/css/management.less" />
<script src="//cdnjs.cloudflare.com/ajax/libs/less.js/2.5.1/less.min.js"></script>

<!-- Bootstrap Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

<link rel="apple-touch-icon" href="/bootstrap/img/apple-touch-icon.png">
<link rel="apple-touch-icon" sizes="72x72" href="/bootstrap/img/apple-touch-icon-72x72.png">
<link rel="apple-touch-icon" sizes="114x114" href="/bootstrap/img/apple-touch-icon-114x114.png">
</head>
======================

<head>
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="description" content="Sandbox for harp-heroku trr-photo-effects" />
<!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
<title>harp-heroku trr-photo-effects</title>

<script src="//cdnjs.cloudflare.com/ajax/libs/less.js/2.5.1/less.min.js"></script>

<!-- Bootstrap Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

<link rel="apple-touch-icon" href="/bootstrap/img/apple-touch-icon.png">
<link rel="apple-touch-icon" sizes="72x72" href="/bootstrap/img/apple-touch-icon-72x72.png">
<link rel="apple-touch-icon" sizes="114x114" href="/bootstrap/img/apple-touch-icon-114x114.png">
</head>

<body class="css-management">
h1 Welcome to harp/photo-effects.
h3 Deployed locally at http://localhost:9000/
h3 Deployed on Heroku at https://harp-photo-effects-94037.herokuapp.com/

<header class="row col-sm-12 css-management-msgs"  style="font-size: .8em; height: 40px;">
<div class="init-status">
</div>
<div class="cycle-status"  cycles="0">
</div>
</header>

<div class="hidden-xs col-sm-2 css-management-profile-column">
<div class="profiles-container">

<div class="profile-container">
<div class="image">
<img class="profile-photo" src="../images/gina_5580042-profile.jpg" />
</div>
<div class="info">
<div class="name">Gina Mina, PhD</div>
<div class="title">Chief Executive Officer</div>
</div>
</div>

</div>
</div>

<div class="col-xs-12 col-sm-10 css-management-bio-column">
<div class="bios-container">

<div class="row bio-container bio-active" active_id = "" active_idx="">
<div class="col-sm-5">
<div class="info">
<div class="name">name</div>
<div class="title">title</div>
<div class="short-bio">short-bio</div>
</div>
</div>
<div class="col-sm-5">
<div class="image">
<img class="profile-photo" src=""/>
</div>
</div>
</div>

</div>
</div>

<!-- jQuery (necessary for plugins) -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script src="../js/ScrollMagic/scrollmagic/uncompressed/ScrollMagic.js"></script>

<!-- script src="../js/exploding-lib.js"></script -->
<!-- script src="../js/management.js"></script -->

</body>
=======================

<html lang="en">

<head>
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="description" content="Sandbox for harp-heroku trr-photo-effects" />
<!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
<title>harp-heroku trr-photo-effects</title>

<!-- Bootstrap Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

<link rel="apple-touch-icon" href="/bootstrap/img/apple-touch-icon.png">
<link rel="apple-touch-icon" sizes="72x72" href="/bootstrap/img/apple-touch-icon-72x72.png">
<link rel="apple-touch-icon" sizes="114x114" href="/bootstrap/img/apple-touch-icon-114x114.png">

<!-- jQuery (necessary for plugins) -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<!-- Latest compiled and minified JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
<script src="../js/ScrollMagic/scrollmagic/uncompressed/ScrollMagic.js"></script>
</head>

<script>
  function statusLog( msg, plugIn) {
    return;
    if ( $( ".init-done" ).length == 0) {
      $( ".init-status" ).append( msg );
    } else {
      if (msg.indexOf("*11-requestAnimationFrame") != -1) {
        var img_src = $('.explode').find('img:first-child').attr('src');
        var name = img_src.slice( img_src.indexOf('/') + 1, img_src.indexOf('_') );
        var cycles = parseInt($( ".cycle-status" ).attr('cycles'));
        if(plugIn.options.direction == 'out') {
          if ( cycles == 2) {
            $( ".cycle-status" ).html( "");
            cycles = 0;
          }
        } else {
          cycles += 1;
        }
        $( ".cycle-status" ).append( "<br />" + "**" + name + "**...");
        $( ".cycle-status" ).attr('cycles', cycles + '');
      }
      $( ".cycle-status" ).append( msg );
    }
  };

  statusLog( "  ..*1-uponLoad*" );

  $(function() {
    // Bind events and initialize plugin
    statusLog( "  ..*2-domReady*" );
    // $('.explode')
      // .on('pixellate-exploded', function() {
      //   var self = this;
      //   setTimeout(function() {
      //     $(self).pixellate('in');
      //   }, 500);
      // })
      // .on('pixellate-imploded', function() {
      //   var self = this;
      //   setTimeout(function() {
      //    $(self).pixellate('out');
      //   }, 2000);
      // })
      // .pixellate();

        // <div class="row bio-container bio-active" active_id = "" active_idx="">
        //   <div class="col-sm-5">
        //     <div class="info">
        //       <div class="name">name</div>
        //       <div class="title">title</div>
        //       <div class="short-bio">
        //         short-bio
        //       </div>
        //     </div>
        //   </div>
        //   <div class="col-sm-5">
        //     <div class="image">
        //       <img class="profile-photo" src=""/>
        //     </div>
        //   </div>
        // </div>

    // 'id', 'bio-idx', 'profile-idx' id="bio-01-jamar"
    $.each( $( '.profile-container' ).toArray(), function( index, el ) {
      img_src = $(el).find('img').attr('src');
      name = img_src.slice( img_src.indexOf('/images') + ('/images'.length + 1), img_src.indexOf('_') );
      $(el).attr( 'id', ('profile-' + (index + '') + '-' + name) );
      $(el).attr('profile-idx', index + '');
      $(el).attr('bio-idx', index + 1 + ''); // first bio is sandbox.
    });

    $.each( $( '.bio-container' ).toArray(), function( index, el ) {
      img_src = $(el).find('img').attr('src');
      name = img_src.slice( img_src.indexOf('/images') + ('/images'.length + 1), img_src.indexOf('_') );
      $(el).attr( 'id', ('bio-' + (index + '') + '-' + name) );
      $(el).attr('bio-idx', index + '');
      $(el).attr('profile-idx', index - 1 + ''); // first bio is sandbox.
      $(el).find('.image').addClass('explode');
    });

    var $active_bio = $('.bio-active'),
        $default_bio = $( $('.bio-container').toArray()[parseInt(defaults.active_profile_idx)] );

    $active_bio.attr('active_id', $default_bio.attr('id'));
    $active_bio.attr('active_idx', $default_bio.attr('bio-idx'));
    $active_bio.find('.name').html($default_bio.find('.name').html());
    $active_bio.find('.title').html($default_bio.find('.title').html());
    $active_bio.find('.short-bio').html($default_bio.find('.short-bio').html());
    $active_bio.find('img').attr('src', $default_bio.find('img').attr('src'));

    $.each( $( '.bio-container' ).find('.image').toArray(), function( index, el ) {
      $(el).addClass('explode');
    });

    var $img_div = $('.explode');
    setTimeout(function() {
      $img_div.pixellate('init'); // fragment image, store in $pixel array as <span> elements.
      $img_div.removeClass('pixellate-lock');
      $( ".init-status" ).addClass('init-done');
      $img_div.pixellate('out');  // explode image via $pixel array, update spans.
      $img_div.pixellate('in');   // recreate from $pixel for initial view.
      // $img_div.data('pixellate-image-el').css('visibility', 'hidden');
      //setTimeout(function() {
      //  $img_div.pixellate('out');
      //  setTimeout(function() {
      //    $img_div.pixellate('in');
      //  }, 2000);
      //}, 1000);
    }, 1000);
    // statusLog( "  ..*3-after domReadyPixellate()*" );
    // $( ".init-status" ).addClass('init-done');

    $.each( $( '.profile-container' ).toArray(), function( index, el ) {
      // alert( index + ": " + $(el).attr('id') );
      //$profile = $('#profile-01-gina');
      $(el).click(function(attribs) {
        var self = $(attribs.currentTarget);
        //alert( 'Clicked on \'' + self.attr('id') + '\'' +
        //       '.  Active halftone profile: ' + $active_bio.attr('active_idx') + ':' + $active_bio.attr('active_id')
        //);
        $source_bio = $( $('.bio-container').toArray() [ parseInt(self.attr('bio-idx')) ] );
        $active_bio.attr('active_id', $source_bio.attr('id'));
        $active_bio.attr('active_idx', $source_bio.attr('bio-idx'));
        $active_bio.find('.name').html($source_bio.find('.name').html());
        $active_bio.find('.title').html($source_bio.find('.title').html());
        $active_bio.find('.short-bio').html($source_bio.find('.short-bio').html());
        $active_bio.find('img').attr('src', $source_bio.find('img').attr('src'));

      });
    });
  });


  var pluginName = 'pixellate',
      defaults = {
        // Grid divisions
        columns: 20,
        rows: 20,

        // Duration of explosion animation
        duration: 1500,

        // Direction of explosion animation ('out', 'in', or 'none')
        direction: 'out',

        // Resize pixels during animation
        scale: true,

        // Coordinates representing the source of the explosion force
        //(e.g. [-1, 1] makes the explodey bits go up and to the right)
        explosionOrigin: [0,0],

        active_profile_idx: "01"
      };
  statusLog( "  ..*4-global data done*" );

  function Plugin(el, options) {
    statusLog( "  ..*5-creating Plugin: for class: " + $(el).attr('class') + "*"); // direction = '" + defaults.direction + "'*");
    this.$el = $(el);
    this.options = $.extend({}, defaults, options);
    this._defaults = defaults;
    this._name = pluginName;

    this.init();
    statusLog( "  ..*6-Plugin init done.*" );
  };

  Plugin.prototype = {
    init: function() {
      // Note: this.$el = '<div class=".explode"'>
      statusLog( "  ..*7-Plugin init*"); // " for this.$el.attr('class'): " + this.$el.attr('class') + "*");
      // this.$el = PlugIn instance's '.explode' container div.
      // this.$el.pixellate-pixel is an array of spans for each image fragment.
      if(!this.$el.find('.pixellate-pixel').length) {
        var $img = this.$el.find('img:first-child'),
            img = new Image();

        this.$el
          .data('pixellate-image-src', $img.attr('src'))
          .data('pixellate-image-el', $img)
          .addClass('pixellate-lock');
        // $img.css('visibility', 'hidden');

        $(img).one('load', $.proxy(this.createPixels, this));

        img.src = this.$el.data('pixellate-image-src');
        if(img.complete) {
          $(img).trigger('load');
        }
      } else {
        this.stylePixels();
      }
    },

    createPixels: function() {
      this.$el.append(new Array((this.options.rows * this.options.columns) + 1).join('<span class="pixellate-pixel"></span>'));
      statusLog( "  ..*9-createPixels: pixellate-pixel[ ].length = '" + this.$el.find('.pixellate-pixel').length + "'*");

      this.stylePixels(true);
      },

    stylePixels: function(initializeStyles) {
      statusLog( "  ..*10-stylePixels(" + this.options.direction +")" + (initializeStyles ? " initializeStyles:" + initializeStyles : "") + "*" );
      var self = this,
          w = this.$el.width(),
          h = this.$el.height(),
          columns = this.options.columns,
          rows = this.options.rows,
          $pixels = this.$el.find('.pixellate-pixel');

      // $('.explode').find('.pixellate-pixel')[0] (length of array = 400)
      // <span class="pixellate-pixel"
      //    style="
      //       position: absolute;
      //       width: 20px; height: 20px;
      //       background-image: url(&quot;./5580042-profile-pictures_halftone-image-generator.png&quot;);
      //       background-size: 400px auto;
      //       backface-visibility: hidden;
      //       left: 0px; top: 0px;
      //       background-position: 0px 0px;
      //       transform: none;
      //       opacity: 1;
      //       transition: all 1500ms ease-in-out 0s;">

      var styles = initializeStyles ? {
        'position': 'absolute',
        'width': (w / columns),
        'height': (h / rows),
        'background-image': 'url('+this.$el.data('pixellate-image-src')+')',
        'background-size': w,
        'backface-visibility': 'hidden'
      } : {};

      for(var idx = 0; idx < $pixels.length; idx++) {
        var pixelStyles = {};

        if(initializeStyles) {
          var x = (idx % columns) * styles.width,
              y = (Math.floor(idx / rows)) * styles.height;

          $.extend(pixelStyles, styles, {
            'left': x,
            'top': y,
            'background-position': (-x)+'px '+(-y)+'px'
          });
        } else {

        if(self.options.direction == 'out') {
          var randX = (Math.random() * 300) - 150 - (self.options.explosionOrigin[0] * 150),
              randY = (Math.random() * 300) - 150 - (self.options.explosionOrigin[1] * 150);

          var transformString = 'translate('+randX+'px, '+randY+'px)';
          if(self.options.scale) {
            transformString += ' scale('+(Math.random() * 1.5 + 0.5)+')';
          }

          $.extend(pixelStyles, {
            'transform': transformString,
            'opacity': 0,
            'transition': self.options.duration+'ms ease-out'
          });
        } else if(self.options.direction == 'in') {
          $.extend(pixelStyles, {
            'transform': 'none',
            'opacity': 1,
            'transition': self.options.duration+'ms ease-in-out'
          });
        }
        }

        $pixels.eq(idx).css(pixelStyles);
      }

      // Use rAF to ensure styles are set before class is modified
      // requestAnimationFrame(function() {
      //   statusLog( "  ..*11-requestAnimationFrame: direction = '" + self.options.direction + "'*", self);
      //   if(self.options.direction == 'out') {
      //     self.$el.removeClass('pixellate-lock');
      //   } else if(self.options.direction == 'in') {
          // self.$el.one('pixellate-imploded', function() {
          //   self.$el.addClass('pixellate-lock');
          // });
      //     self.$el.addClass('pixellate-lock');
      //   }
      // });

      // Fire plugin events after animation completes
      // TODO: Use transition events when supported
      // setTimeout(function() {
      //   if(self.options.direction == 'out')
      //     self.$el.trigger('pixellate-exploded');
      //   else if(self.options.direction == 'in')
      //     self.$el.trigger('pixellate-imploded');
      // }, this.options.duration);
    }
  };

  $.fn[ pluginName ] = function ( options ) {
    return this.each(function() {
      // Note: this = '<div class=".explode"'>
      if ( !$.data( this, "plugin_" + pluginName ) ) {
        statusLog( "  ..*5b: $.fn[ " + pluginName + " ]*" );
        $.data( this, "plugin_" + pluginName, new Plugin( this, options ) );
      } else if(typeof options === 'string') {
        statusLog( "  ..*5c: $.fn[ " + pluginName + " ] direction: " + options + "*" );
        $.data( this, "plugin_" + pluginName ).options.direction = options;
        $.data( this, "plugin_" + pluginName ).init();
      }
    });
  };


  // requestAnimationFrame polyfill by Erik Möller. fixes from Paul Irish and Tino Zijdel
  // MIT license
  var lastTime = 0;
  var vendors = ['ms', 'moz', 'webkit', 'o'];
  for(var x = 0; x < vendors.length && !window.requestAnimationFrame; ++x) {
    window.requestAnimationFrame = window[vendors[x]+'RequestAnimationFrame'];
    window.cancelAnimationFrame = window[vendors[x]+'CancelAnimationFrame'] || window[vendors[x]+'CancelRequestAnimationFrame'];
  }

  if (!window.requestAnimationFrame)
    window.requestAnimationFrame = function(callback, element) {
        var currTime = new Date().getTime();
        var timeToCall = Math.max(0, 16 - (currTime - lastTime));
        var id = window.setTimeout(function() { callback(currTime + timeToCall); },
          timeToCall);
        lastTime = currTime + timeToCall;
        return id;
    };

  if (!window.cancelAnimationFrame)
    window.cancelAnimationFrame = function(id) {
        clearTimeout(id);
    };
  //statusLog( "  ..*12: Add window.request/cancelAnimationFrame()*" );
</script>
