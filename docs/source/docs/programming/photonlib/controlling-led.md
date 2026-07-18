# Controlling LEDs

You can control the vision LEDs of supported hardware via PhotonLib using the `setLED()` method on a `PhotonCamera` instance. In Java, C++, and Python, an LED mode enum class is provided to choose values from. These values include `kOff`, `kOn`, `kBlink` (or `kBLINK` in Python), and `kDefault` (or `kDEFAULT` in Python). `kDefault` uses the default LED value from the selected pipeline.

```{eval-rst}
.. tab-set-code::
   .. code-block:: java

      // Blink the LEDs.
      camera.setLED(VisionLEDMode.kBlink);

   .. code-block:: c++

      // Blink the LEDs.
      camera.SetLED(photonlib::VisionLEDMode::kBlink);

   .. code-block:: python
        .. code-block:: java

      // Blink the LEDs.
      camera.setLED(VisionLEDMode.kBlink);

   .. code-block:: c++

      // Blink the LEDs.
      camera.SetLED(photonlib::VisionLEDMode::kBlink);

   .. code-block:: python

        # Blink the LEDs.
        camera.setLED(photonvision.LEDMode.kBLINK)

```
