# Prueba_Andreani
Prueba tecnica -andreani

Una vez que se corra el docker-compose up

si la base de datos no esta persisitida : 

Ejecutar : 

/opt/mssql-tools/bin/sqlcmd -S localhost -U SA -P Pass@word



USE [master]
GO
CREATE DATABASE [Prueba_Andreani]
GO

CREATE TABLE [dbo].[Pedido](	[Id] [int] IDENTITY(1,1) NOT NULL,	[calle] [nvarchar](50) NOT NULL,	[numero] [nvarchar](50) NOT NULL,	[ciudad] [nvarchar](50) NOT NULL,	[provincia] [nvarchar](50) NOT NULL,	[pais] [nvarchar](50) NOT NULL,[latitud] [nvarchar](100) NULL,	[longitud] [nvarchar](100) NULL, CONSTRAINT [PK_Pedido] PRIMARY KEY CLUSTERED (	[Id] ASC)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON) ON [PRIMARY]) ON [PRIMARY]
GO
