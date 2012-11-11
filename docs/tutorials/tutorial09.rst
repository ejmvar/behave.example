.. _id.tutorial09:

Tutorial 9: Use Background
==============================================================================

:Goal: Use the ``Background`` concept to execute a number of steps before each scenario.

.. hint::
    This example is based on the `Ninja Survival Rate`_ examples
    from [SecretNinja10]_.

.. _`Ninja Survival Rate`: https://github.com/davedf/cuke4ninja/tree/master/src/ruby/NinjaSurvivalRate/features


Write the Feature Test
------------------------

.. literalinclude:: ../../features/tutorial09_background.feature
    :language: gherkin
    :prepend: # file:features/tutorial09_background.feature


Provide the Test Automation
-----------------------------

.. literalinclude:: ../../features/steps/step_tutorial02.py
    :prepend:   # file:features/steps/step_tutorial02.py
    :append:    ...
    :language: python
    :lines:  1, 22-25, 52-65


Provide the Domain Model
-----------------------------

.. literalinclude:: ../../features/steps/step_tutorial02.py
    :prepend:   # file:features/steps/step_tutorial02.py
    :language: python
    :lines:  26-51

Run the Feature Test
-----------------------------

When you run this feature test with the background functionality:

.. command-output:: behave ../features/tutorial09_background.feature
    :shell: