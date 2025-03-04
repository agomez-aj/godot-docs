:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/SubViewportContainer.xml.

.. _class_SubViewportContainer:

SubViewportContainer
====================

**Inherits:** :ref:`Container<class_Container>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

Control for holding :ref:`SubViewport<class_SubViewport>`\ s.

.. rst-class:: classref-introduction-group

Description
-----------

A :ref:`Container<class_Container>` node that holds a :ref:`SubViewport<class_SubViewport>`. It uses the :ref:`SubViewport<class_SubViewport>`'s size as minimum size, unless :ref:`stretch<class_SubViewportContainer_property_stretch>` is enabled.

\ **Note:** Changing a SubViewportContainer's :ref:`Control.scale<class_Control_property_scale>` will cause its contents to appear distorted. To change its visual size without causing distortion, adjust the node's margins instead (if it's not already in a container).

\ **Note:** The SubViewportContainer forwards mouse-enter and mouse-exit notifications to its sub-viewports.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------+---------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>` | :ref:`stretch<class_SubViewportContainer_property_stretch>`               | ``false`` |
   +-------------------------+---------------------------------------------------------------------------+-----------+
   | :ref:`int<class_int>`   | :ref:`stretch_shrink<class_SubViewportContainer_property_stretch_shrink>` | ``1``     |
   +-------------------------+---------------------------------------------------------------------------+-----------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_SubViewportContainer_property_stretch:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **stretch** = ``false``

.. rst-class:: classref-property-setget

- void **set_stretch** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_stretch_enabled** **(** **)**

If ``true``, the sub-viewport will be automatically resized to the control's size.

.. rst-class:: classref-item-separator

----

.. _class_SubViewportContainer_property_stretch_shrink:

.. rst-class:: classref-property

:ref:`int<class_int>` **stretch_shrink** = ``1``

.. rst-class:: classref-property-setget

- void **set_stretch_shrink** **(** :ref:`int<class_int>` value **)**
- :ref:`int<class_int>` **get_stretch_shrink** **(** **)**

Divides the sub-viewport's effective resolution by this value while preserving its scale. This can be used to speed up rendering.

For example, a 1280×720 sub-viewport with :ref:`stretch_shrink<class_SubViewportContainer_property_stretch_shrink>` set to ``2`` will be rendered at 640×360 while occupying the same size in the container.

\ **Note:** :ref:`stretch<class_SubViewportContainer_property_stretch>` must be ``true`` for this property to work.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
