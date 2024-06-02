## Instalación y configuración de Zerotier.

Descarga Zerotier de su página oficial --> [Descarga Aquí](https://www.zerotier.com/download/)

### **Paso 1: Instalación de Agente.** 

En este caso lo vamos a instalar en un SO debian. 

```
curl -s https://install.zerotier.com | sudo bash
```

![image](https://github.com/Buzziexit/Zurgshield/assets/114906778/f293039b-76b3-4e79-8476-037a63578b06)


### Paso 2: Crear una red en Zerotier. 

Primero debes crearte una cuenta. Una vez tengas tu usario puedes seguir los siguientes pasos.

1. Pulsamos en create a Network

![image](https://github.com/Buzziexit/Zurgshield/assets/114906778/c50cdd80-f267-4d5a-a42d-0f1d48646352)

2. Configuramos la red

![image](https://github.com/Buzziexit/Zurgshield/assets/114906778/e49ad1a0-b272-4758-93b4-d7f15e7ff972)

Podemos cambiar el rango de IP o dejarlo por defecto:

![image](https://github.com/Buzziexit/Zurgshield/assets/114906778/4cf0ef44-22c2-42ae-9d35-ac757b2a670e)

### Paso 3: Unirse a la red

En el agente ejecutamos el siguiente comando:

```
zerotier-cli join <Network ID>
```

Esto lo encontramos:

![image](https://github.com/Buzziexit/Zurgshield/assets/114906778/c3380659-8096-4e5f-b8ac-629b84bd9a2b)


![image](https://github.com/Buzziexit/Zurgshield/assets/114906778/ba0d1ef1-1294-499e-b1fd-31e3fc0fd914)

Y ahora desde nuestra central de Zerotier tenemos que autorizar este dispositivo.

![image](https://github.com/Buzziexit/Zurgshield/assets/114906778/1182f93b-991d-41ac-99f7-de342eebda42)

Autorizamos y nos da una ip automaticamente que podemos cambiar si queremos.

![image](https://github.com/Buzziexit/Zurgshield/assets/114906778/6b3abb98-f6b0-48e3-80ea-cfa47f5082f8)


