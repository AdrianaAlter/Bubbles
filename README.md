# Bubbles

Bubbles is a demonstration of CSS3 techniques.  It uses pseudo elements and radial gradients to create the effect of translucent, three-dimensional bubbles, and deploys three different keyframe animation technology to make them move realistically.  For example, the following keyframe sequence causes the bubbles to start out slightly flattened, and gradually become fully circular as they drift upwards:

<pre><code>
  @keyframes squish {
    0% { transform: scaleY(0.5) scaleX(1.5); }
    15% { transform: scaleY(0.75) scaleX(1.25); }
    20% { transform: scaleY(1.05) scaleX(0.95); }
    25%, 35%, 45%, 55%, 65%, 75%, 85%, 95% {
      transform: scale(.9);
    }
    30%, 40%, 50%, 60%, 70%, 80%, 90%, 100% {
      transform: scale(1);
    }
  }
</code></pre>

The spinning text at the top left and bottom right corners showcases CSS transforms on all three axes.  Mousing over any individual bubble will restart its animation cycle, essentially meaning that you can adjust the bubbles' distribution on your screen.  If you catch the bubbles at the top of the screen, you can even pop them!  To fill your own computer screen with bubbles, visit http://adrianaalter.github.io/Bubbles/.

<img src="./images/bubbles.png"></img>
