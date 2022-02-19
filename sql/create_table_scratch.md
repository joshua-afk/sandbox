### MS SQL
-------------------------------------------------

USE [database_name]
GO

SET ANSI_NULLS ON
GO

SET QUOTED_IDENTIFIER ON
GO

SET ANSI_PADDING ON
GO

CREATE TABLE [dbo].[table_name](
	Id INT IDENTITY(1,1) NOT NULL,
	FirstName VARCHAR(50) NULL,
	LastName VARCHAR(50) NULL,
	Income FLOAT NULL,
	DateRow DATETIME NULL,
	SomeOtherId INT NULL,

  __NOTE: DF means default__
  Active BIT NOT NULL CONSTRAINT [DF_table_name_Active] DEFAULT(1),

  __NOTE: PK means primary key__
  CONSTRAINT [PK_table_name_Id] PRIMARY KEY CLUSTERED
	(
			[Id]
		  ) ON [PRIMARY]
	) ON [PRIMARY]
GO


