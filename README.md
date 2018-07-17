# ESP32_FreeRTOS_Queue

The Project demonstrates FreeRTOS Queue on ESP32 with AWS IoT


# Amazon Web Services IoT MQTT Subscribe/Publish Example

This is an adaptation of the [AWS IoT C SDK](https://github.com/aws/aws-iot-device-sdk-embedded-C) "subscribe_publish" example for ESP-IDF.



# Monitoring MQTT Data from the device

After flashing the example on ESP32, it should connect to Amazon and start subscribing/publishing MQTT data.

The example code publishes MQTT data to the topic `esp`. Amazon provides a web interface to subscribe to MQTT topics for testing:

* On the AWS IoT console, click "MQTT Client" near the top-right.
* Click "Generate Client ID" to generate a random client ID.
* Click "Connect"

One connection succeeds, you can subscribe to the data published by the ESP32:

* Click "Subscribe to Topic"
* Enter "Subscription Topic" 'esp`
* Click "Subscribe"

... you should see MQTT data published from the running example.

To publish data back to the device:

* Click "Publish to Topic"
* Enter "Publish Topic" `esp`
* Enter a message in the payload field
* Click Publish
