# Examen Final Microservicios:


## Archivo "infra-compose.yml":
-El archivo "infra-compose.yml" contiene todas las dependencias necesarias para ejecutar los microservicios.
-La ubicación del archivo es:
	WksMicroserviciosSpringCloud_exam_01\docker\infra-compose.yml
-Ejecutar el siguiente comando para levantar todo:
docker-compose --profile core --file infra-compose.yml up -d --build 

## Inserta Data Inicial en la BD:
-A continuación indico los insert necesarios que se debe agregar a la Base de Datos:
	-Para la base de datos inventorydb se debe ejecutar los siguientes insert:
		INSERT INTO warehouses (id, name, address, warehouse_type) VALUES (1000, 'Centro de Distribución Norte', 'Av. Universitaria 4500, Los Olivos', 'DISTRIBUTION_CENTER');
		INSERT INTO warehouses (id, name, address, warehouse_type) VALUES (2000, 'Centro de Distribución Sur', 'Av. El Sol 980, Villa El Salvador', 'DISTRIBUTION_CENTER');
		INSERT INTO warehouses (id, name, address, warehouse_type) VALUES (3000, 'Almacén de Miraflores', 'Calle Berlín 320, Miraflores', 'RETAIL');
		INSERT INTO warehouses (id, name, address, warehouse_type) VALUES (4000, 'Almacén de San Isidro', 'Av. Javier Prado Oeste 2100, San Isidro', 'RETAIL');
		INSERT INTO warehouses (id, name, address, warehouse_type) VALUES (5000, 'Depósito Callao (Puerto)', 'Zona Portuaria del Callao, Callao', 'IMPORT_EXPORT');
		INSERT INTO warehouses (id, name, address, warehouse_type) VALUES (6000, 'Almacén de Productos Frágiles', 'Av. Nicolás Ayllón 5400, Ate', 'FRAGILE_GOODS');
		INSERT INTO warehouses (id, name, address, warehouse_type) VALUES (7000, 'Almacén de Alta Rotación', 'Av. México 1200, La Victoria', 'HIGH_ROTATION');
		INSERT INTO warehouses (id, name, address, warehouse_type) VALUES (8000, 'Almacén de Baja Rotación', 'Panamericana Sur Km 35, Lurín', 'LOW_ROTATION');
	-Para la base de datos inventorydb se debe ejecutar los siguientes insert:
		INSERT INTO shipping_companies (id, name, phone_number, email, web_site) VALUES (1000001, 'Serpost', '51960000001', 'contacto@serpost.com.pe', 'https://www.serpost.com.pe');
		INSERT INTO shipping_companies (id, name, phone_number, email, web_site) VALUES (1000002, 'Olva Courier', '51960000002', 'atencionalcliente@olva.pe', 'https://www.olva.pe');
		INSERT INTO shipping_companies (id, name, phone_number, email, web_site) VALUES (1000003, 'Shalom', '51960000003', 'contacto@shalom.com.pe', 'https://www.shalom.com.pe');
		INSERT INTO shipping_companies (id, name, phone_number, email, web_site) VALUES (1000004, 'Marvisur', '51960000004', 'informes@marvisur.com', 'https://www.marvisur.com');
		INSERT INTO shipping_companies (id, name, phone_number, email, web_site) VALUES (1000005, 'Cruz del Sur Cargo', '51960000005', 'cargo@cruzdelsur.com.pe', 'https://www.cruzdelsurcargo.com.pe');
		INSERT INTO shipping_companies (id, name, phone_number, email, web_site) VALUES (1000006, 'Flores Cargo', '51960000006', 'servicioalcliente@florescargo.com', 'https://www.florescargo.com');
		INSERT INTO shipping_companies (id, name, phone_number, email, web_site) VALUES (1000007, 'FedEx', '51960000007', 'support@fedex.com', 'https://www.fedex.com');
		INSERT INTO shipping_companies (id, name, phone_number, email, web_site) VALUES (1000008, 'DHL', '51960000008', 'customer.service@dhl.com', 'https://www.dhl.com');
		INSERT INTO shipping_companies (id, name, phone_number, email, web_site) VALUES (1000009, 'Amazon Logistics', '51960000009', 'logistics@amazon.com', 'https://logistics.amazon.com');
		INSERT INTO shipping_companies (id, name, phone_number, email, web_site) VALUES (1000010, 'UPS', '51960000010', 'customer.service@ups.com', 'https://www.ups.com');


## Para levantar los microservicios desde el IDE ver el word 13. Microservicios levantados desde IDE.docx:
PROYECTOS Y PERFILES LEVANTADOS:
  api-order-service-v1              --> dev
  api-payment-service-v1            --> dev 
  api-payment-service-v2            --> dev 
  api-inventory-service-v1          --> dev
  api-shipment-service-v1           --> dev
  api-order-orchestrator-service-v1 --> RestClient,dev
  api-order-query-service-v1        --> dev

## Enlaces: 
-Repositorio GITHUB config-server:  https://github.com/mirkocarrrasco/2026_I_SCL_ESTUDIANTES_EXAM/tree/main/infra/config-server-properties
-Repositorio GITHUB Microservicios: https://github.com/mirkocarrrasco/2026_I_SCL_ESTUDIANTES_EXAM_SIN-SEGURIDAD 
-Repositorio GITHUB Documentación y evidencias: https://github.com/mirkocarrrasco/2026_I_SCL_ESTUDIANTES_EXAM_SIN-SEGURIDAD/tree/main/Documentacion
-Repositorio Google Drive con Documentación y evidencias: https://drive.google.com/drive/folders/165FtG2OmbLATgXboXyHCI6wb2fSA1lQG
-Repositorio Google Drive con Video de evidencia de las Pruebas: 
  -Video Pruebas Flujo Principal.zip:          https://drive.google.com/file/d/1zFckGNMe835VD0fX0tZtFdIfgm5sJkqF/view?usp=drive_link
  -Video Pruebas Flujo con Compensaciones.zip: https://drive.google.com/file/d/1slZPJVE1hcJMAoPVA95Ot2NSsSGNz4HK/view?usp=drive_link


