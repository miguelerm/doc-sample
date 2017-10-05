# Servicio usuarios

Este es un servicio SOAP y su descipcion en WSDL se encuentra en este link [UsuariosServicio.wsdl](UsuariosServicio.wsdl).

La mayoría de IDES generan un proxy que pueden consumir en el lenguaje y plataforma de su preferencia.

Este servicio se compone de los siguientes metodos:

* ObtenerUsuarios

## Obtener Usuarios

Obtiene todos los usuarios

### SOAP 1.1

The following is a sample SOAP 1.1 request and response. The placeholders shown need to be replaced with actual values.

```
POST /UsuariosServicio.asmx HTTP/1.1
Host: localhost
Content-Type: text/xml; charset=utf-8
Content-Length: length
SOAPAction: "https://miguelerm.github.io/servicios/ObtenerUsuarios"

<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ObtenerUsuarios xmlns="https://miguelerm.github.io/servicios/" />
  </soap:Body>
</soap:Envelope>
```

```
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Content-Length: length

<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ObtenerUsuariosResponse xmlns="https://miguelerm.github.io/servicios/">
      <ObtenerUsuariosResult>
        <UsuarioModelo>
          <Id>int</Id>
          <Nombre>string</Nombre>
        </UsuarioModelo>
        <UsuarioModelo>
          <Id>int</Id>
          <Nombre>string</Nombre>
        </UsuarioModelo>
      </ObtenerUsuariosResult>
    </ObtenerUsuariosResponse>
  </soap:Body>
</soap:Envelope>
```

### SOAP 1.2

The following is a sample SOAP 1.2 request and response. The placeholders shown need to be replaced with actual values.

```
POST /UsuariosServicio.asmx HTTP/1.1
Host: localhost
Content-Type: application/soap+xml; charset=utf-8
Content-Length: length

<?xml version="1.0" encoding="utf-8"?>
<soap12:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap12="http://www.w3.org/2003/05/soap-envelope">
  <soap12:Body>
    <ObtenerUsuarios xmlns="https://miguelerm.github.io/servicios/" />
  </soap12:Body>
</soap12:Envelope>
```

```
HTTP/1.1 200 OK
Content-Type: application/soap+xml; charset=utf-8
Content-Length: length

<?xml version="1.0" encoding="utf-8"?>
<soap12:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap12="http://www.w3.org/2003/05/soap-envelope">
  <soap12:Body>
    <ObtenerUsuariosResponse xmlns="https://miguelerm.github.io/servicios/">
      <ObtenerUsuariosResult>
        <UsuarioModelo>
          <Id>int</Id>
          <Nombre>string</Nombre>
        </UsuarioModelo>
        <UsuarioModelo>
          <Id>int</Id>
          <Nombre>string</Nombre>
        </UsuarioModelo>
      </ObtenerUsuariosResult>
    </ObtenerUsuariosResponse>
  </soap12:Body>
</soap12:Envelope>
```

### HTTP POST

The following is a sample HTTP POST request and response. The placeholders shown need to be replaced with actual values.

```
POST /UsuariosServicio.asmx/ObtenerUsuarios HTTP/1.1
Host: localhost
Content-Type: application/x-www-form-urlencoded
Content-Length: length
```

```
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Content-Length: length

<?xml version="1.0" encoding="utf-8"?>
<ArrayOfUsuarioModelo xmlns="https://miguelerm.github.io/servicios/">
  <UsuarioModelo>
    <Id>int</Id>
    <Nombre>string</Nombre>
  </UsuarioModelo>
  <UsuarioModelo>
    <Id>int</Id>
    <Nombre>string</Nombre>
  </UsuarioModelo>
</ArrayOfUsuarioModelo>
```

