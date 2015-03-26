Work in progress
================

This document will eventually describe the process of implementing
the BlogBundle.

Routing
-------

Register the routes in config.yml

.. code-block:: php

    cmf_routing:
        dynamic:
            ...
            controllers_by_class:
                Symfony\Cmf\Bundle\BlogBundle\Doctrine\Phpcr\Blog: cmf_blog.blog_controller:listAction
                Symfony\Cmf\Bundle\BlogBundle\Doctrine\Phpcr\Post: cmf_blog.blog_controller:viewPostAction
                Symfony\Cmf\Bundle\BlogBundle\Doctrine\Phpcr\Tag: cmf_blog.blog_controller:listAction
