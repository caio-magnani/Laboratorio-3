# Mapeamento Modelo Relacional
NaturalPersonUser(@id, CPF, Wallet, [idUser]() )

Student(@id, SSN, Address, CollegeProgram, BankAccount, [idNaturalPersonUser]() )

Teacher(@id, department, BankAccount, [idNaturalPersonUser]() )

User(@id, Name, Email, Password)

LegalPersonUser(@id, CNPJ, [idUser]() , [idInstitution]() )

Partner(@id, Name, [idOffer]() )

Offer(@id, Name, Cost, [idCoupon]() )

Institution(@id, Name, [idStudent]() , [idOffer]() )

History(@id, Name, [idBankAccount]() )

BankAccount(@id, Coins)

[back](../README.md)