# API de Cadastro de Leads

## Descrição

Este endpoint é responsável por cadastrar leads no sistema, com informações pessoais, acadêmicas e de campanha de marketing.

### Endpoint

`POST /api/contact-form`

### Cabeçalhos (Headers)

- **Content-Type:** `application/json`
- **Authorization:** `Basic {token_base64}`

  O cabeçalho de autenticação Basic requer a codificação em Base64 do `username:password`. Insomnia faz isso automaticamente ao configurar a autenticação Basic.

---

## Parâmetros da Requisição

### Corpo (Body) - JSON

A requisição deve enviar os seguintes campos no corpo (em formato JSON):

```json
{
  "fullName": "John Doe", // Nome completo do lead
  "email": "johndoe@example.com", // E-mail do lead
  "phoneNumber": "+5511999999999", // Telefone em formato internacional
  "unitId": "dsadsadasdsadasd", // ID da unidade ou referência interna
  "birthDate": "1990-01-01", // Data de nascimento (AAAA-MM-DD)
  "educationInstitution": "University Name", // Nome da instituição de ensino
  "educationCourse": "Computer Science", // Curso do lead
  "educationCourseStartDate": "Em até 30 dias", // Data de início do curso
  "desiredMoveInDate": "Em até 30 dias", // Data pretendida para mudança (opcional)
  "educationAcademicMoment": "Calouro", // Momento acadêmico (Calouro, Veterano, etc.)
  "leadSource": "WebSite", // Origem do lead
  "leadStatus": "1 - Novo", // Status do lead (1 - Novo)
  "gclid": "EAIaIQobChMIv6iqvbHqhgMVCVpIAB1o_AO0EAAYASAAEgL5SPD_BwE", // Google Click ID
  "utmSource": "social", // Fonte da campanha de marketing
  "utmMedium": "cpm", // Meio da campanha de marketing (cpm)
  "utmCampaign": "campanha-cadastro-433-video", // Nome da campanha de marketing
  "utmTerm": "120210622944130162", // Termo de busca da campanha
  "utmContent": "120210622944140162" // Conteúdo da campanha
}
```

# API Pré reserva

## Descrição

Este endpoint é responsável por cadastrar uma pré reserva no sistema, com informações pessoais, acadêmicas e de campanha de marketing.

### Endpoint

`POST /api/pre-booking`

### Cabeçalhos (Headers)

- **Content-Type:** `application/json`
- **Authorization:** `Basic {token_base64}`

  O cabeçalho de autenticação Basic requer a codificação em Base64 do `username:password`. Insomnia faz isso automaticamente ao configurar a autenticação Basic.

---

## Parâmetros da Requisição

### Corpo (Body) - JSON

A requisição deve enviar os seguintes campos no corpo (em formato JSON):

```json


 {
    "fullName": "John Doe",  // Nome completo
    "email": "johndoe@example.com",  // E-mail
    "phoneNumber": "+5511999999999",  // Telefone
    "unitId": "dsdasdsad",  // id da Unidade
    "birthDate": "1990-01-01",  // Data de nascimento
    "cpf": "123.456.789-00",  // CPF (opcional)
    "document": "123456789",  // RG ou Passaporte
    "nationality": "Brazilian",  // Nacionalidade
    "educationAcademicMoment": " Calouro", // Momento da vida acadêmica
    "educationLevel": "Ensino Médio", // Grau de escolaridade
    "educationGraduationYear": "2º semestre", // Ano de graduação
    "educationInstitution": "University Name",  // Instituição de ensino
    "educationCourse": "Computer Science",  // Curso
    "addressCountry": "Brazil",  // País
    "addressStreet": "Street Name",  // Rua
    "addressNumber": "123",  // Número
    "addressComplement": "Apt 45",  // Complemento (opcional)
    "addressZipCode": "12345-678",  // CEP
    "addressNeighborhood": "Neighborhood Name",  // Bairro
    "addressCity": "City Name",  // Cidade
    "addressState": "SP",  // Estado
    "desiredMoveInDate": "Em até 30 dias",  // Data de mudança pretendida (opcional)
    "contractEndDate":"2024-01-31"  // Data final do contrato
    "typologyId": "dsadasdada",  // Tipo de quarto
    "havePet": false,  // Possui pet?
    "discountCoupon": "DISCOUNT2024",  // Cupom de desconto (opcional)
    "financialResponsible": {  // Responsável financeiro
      "fullName": "Jane Doe",  // Nome completo
      "email": "janedoe@example.com",  // E-mail
      "phone": "+5511999999999",  // Telefone
      "birthDate": "1970-01-01",  // Data de nascimento
      "cpf": "987.654.321-00",  // CPF (opcional)
      "document": "987654321",  // RG ou Passaporte
      "nationality": "Brazilian",  // Nacionalidade
      "addressCountry": "Brazil",  // País
      "addressStreet": "Street Name",  // Rua
      "addressNumber": "123",  // Número
      "addressComplement": "Apt 45",  // Complemento (opcional)
      "addressZipCode": "12345-678",  // CEP
      "addressNeighborhood": "Neighborhood Name",  // Bairro
      "addressCity": "City Name",  // Cidade
      "addressState": "SP"  // Estado
    },
	"gclid":"Cj0KCQjwq_G1BhCSARIsACc7Nxriqe46pu111XiKm7UccnPp_fw3tfpBWl-WDlbAmlbadmW-7kLkL2oaAnjjEALw_wcB",
	"utmSource":"",
	"utmMedium":"",
	"utmCampaign":"",
	"utmTerm":"",
	"utmContent":""
  }
```
