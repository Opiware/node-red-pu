
\node-red modbus rtu tcp\

AN32 Node-RED example of Modbus / TCP ( https://www.netio-products.com/en/application-notes/an32-node-red-example-of-modbus-tcp-communication-with-netio-4x-powercable )


\FSM Reset On State INIT\
FSM State On Reset INIT #93 ( https://github.com/BiancoRoyal/node-red-contrib-modbus/issues/93 )
tinktonk: We have the exact same problem, usually working but it looks like we have some problem with the serial connection. If we reset the serial port it starts working again.

biancode: Please, try to give some delay in time for the device to connect if you are using the inject node.

Json file: node-red_rs485_modbus_test.json, modbus-write has e errors:
22 Oct 13:53:34 - [warn] [modbus-write:54bb4178.69fc68] FSM Reset On State INIT
22 Oct 13:53:30 - [warn] [modbus-write:54bb4178.69fc68] FSM Reset On State QUEUEING
22 Oct 13:55:13 - [error] [modbus-write:54bb4178.69fc68] Error: FSM Not Ready To Write At state INIT

===============================================================================
