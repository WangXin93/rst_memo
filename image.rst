Images
######################################################################

The image directive looks very similar to the label syntax. The image directive is just one of the many directives that is supported by reStructuredText. For the time being, **It is enough to know that the directives start with two periods followed by a space, the name of the directive, and two colons**:

.. image:: python.png

To specify the width and height or the scale (in percent) of the iamge:

.. image:: python.png
    :width: 150
    :height: 100


.. image:: python.png
    :scale: 200


In addition to the image direction, there is also the `figure` directive. The difference is that `figure` adds a caption to the image:

.. figure:: python.png
    :scale: 200

    The Python logo

