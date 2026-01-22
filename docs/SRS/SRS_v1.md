\# SRS\_v1 – Especificación de Requisitos del Software



\## 1. Introducción



Este documento describe los requisitos del sistema \*\*Gestión Básica de Turnos\*\*, el cual permite registrar, consultar y administrar turnos de manera sencilla.  

El presente documento forma parte de la \*\*Baseline v1.0\*\* y sirve como referencia para el diseño, desarrollo y pruebas del sistema.



---



\## 2. Alcance del sistema



El sistema permitirá:

\- Registrar turnos de usuarios.

\- Consultar turnos existentes.

\- Administrar el estado de los turnos.

El sistema está orientado a un escenario simple, con fines académicos y de práctica en gestión de configuración.



---



\## 3. Requisitos Funcionales (RF)



\*\*RF-001:\*\*  

El sistema debe permitir registrar un nuevo turno ingresando nombre del usuario, fecha y hora.



\*\*RF-002:\*\*  

El sistema debe permitir listar todos los turnos registrados.



\*\*RF-003:\*\*  

El sistema debe permitir consultar un turno específico mediante un identificador.



\*\*RF-004:\*\*  

El sistema debe permitir actualizar el estado de un turno (pendiente, atendido, cancelado).



---



\## 4. Requisitos No Funcionales (RNF)



\*\*RNF-001 (Usabilidad):\*\*  

El sistema debe ser fácil de usar y comprensible para un usuario sin conocimientos técnicos.



\*\*RNF-002 (Mantenibilidad):\*\*  

El código debe estar estructurado de forma clara y documentada para facilitar futuros cambios.



---



\## 5. Suposiciones y restricciones



\- El sistema se ejecuta en un entorno local.

\- No se consideran aspectos de seguridad avanzada (autenticación o cifrado).

\- El alcance se limita a una implementación mínima funcional.



---



\## 6. Control de versiones



\- Versión: v1.0  

\- Estado: Aprobado (Baseline v1.0)


**RF-007:**  
El sistema debe permitir eliminar un turno existente mediante su identificador.



