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
	[Id] [int] IDENTITY(1,1) NOT NULL,
	[FirstName] [varchar](50) NULL,
	[LastName] [varchar](50) NULL,
	[Income] [float] NULL,
	[DateRow] [datetime] NULL,
	[SomeOtherId] [int] NULL,

  __NOTE: DF means default__
  Active BIT NOT NULL CONSTRAINT [DF_table_name_Active] DEFAULT(1),

  __NOTE: PK means primary key__
  CONSTRAINT [PK_table_name_Id] PRIMARY KEY CLUSTERED
GO


