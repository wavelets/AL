Documentation
====================

al
----

al.instance_strategies
^^^^^^^^^^^^^^^^^^^^^^

.. automodule:: al.instance_strategies
   :members:

al.learning_curve
^^^^^^^^^^^^^^^^^

.. automodule:: al.learning_curve
   :members:

front_end.cl
------------

.. automodule:: front_end.cl.run_al_cl
   :members:

Examples
^^^^^^^^
   The following code runs :mod:`front_end.cl.run_al_cl` with the following parameters:

   * number of trials - 5
   * strategy - rand
   * bootstrap - 10
   * budget - 500
   * step size - 10
   * subpool - 250
   * data paths - ../../../data/imdb-binary-pool-mindf5-ng11 ../../../data/imdb-binary-test-mindf5-ng11

   .. code-block:: python

      python run_al_cl.py -c MultinomialNB -nt 5 -st rand -bs 10 -b 500 -sz 10 -sp 250 -d ../../../data/imdb-binary-pool-mindf5-ng11 ../../../data/imdb-binary-test-mindf5-ng11

   *The output of this code is:*

   *Status:*

   .. code-block:: python

      Loading took 17.88s.

      trial 0
      trial 1
      trial 2
      trial 3
      trial 4

   *Data output is placed in a file in your current working directory. The
   default filename is avg_results.txt.*

   *Sample Data Output:*

   .. code-block:: python

      rand
      accuracy
      train size,mean
      10,0.557016
      20,0.538432
      30,0.534664
      40,0.575320
      50,0.651672
      60,0.621416
      70,0.670400
      80,0.645680
      90,0.659520
      100,0.610160
      110,0.658024

   *Plot Image:*

   .. image:: _images/run1.png
      :width: 50%

front_end.gui
-------------

.. automodule:: front_end.gui.run_al_gui
   :members:

Examples
^^^^^^^^

   The following provides an in-depth look at a sample run of :mod:`front_end.gui.run_al_gui`

   .. code-block:: python

      python run_al_gui.py

   *GUI Main Window (with all values reset)*

   .. image:: _images/gui_main.png
      :width: 80%

   *Setting up the gui to run the following equivalent run of the command line interface:*

   .. code-block:: python

      python run_al_cl.py -c MultinomialNB -d /home/geet/Dropbox/Research/Bilgic/data/20_newsgroups_train /home/geet/Dropbox/Research/Bilgic/data/20_newsgroups_train hash -nt 5 -st rand -bs 10 -b 500 -sz 10 -sp 250

   *Choose train and test data files:*

   .. image:: _images/choose_data.png
      :width: 50%
      :align: left

   .. image:: _images/loaded_gui.png
      :width: 80%

   *Edit parameters to match specified run:*

   .. image:: _images/edit_parameters.png
      :width: 20%

   *Choose MultinomialNB and rand as the classifier-strategy combination:*

   .. image:: _images/choose_clas_strat.png
      :width: 30%

   *Run terminal output:*

   .. code-block:: python

      python run_al_cl.py -pf MultinomialNB-rand -c MultinomialNB -d /home/geet/Dropbox/Research/Bilgic/data/20_newsgroups_train /home/geet/Dropbox/Research/Bilgic/data/20_newsgroups_train hash -nt 5 -st rand -bs 10 -b 500 -sz 10 -sp 250
      trial 0
      trial 1
      trial 2
      trial 3
      trial 4

   *Show plots when done:*

   .. image:: _images/show_plots.png
      :width: 50%

utils.utils
-----------

.. automodule:: utils.utils
   :members:
