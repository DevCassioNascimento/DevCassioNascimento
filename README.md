<div align="center">

  <!-- BANNER / HEADER COM AS CORES DO SITE -->
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0F0D0B&height=150&section=header&text=CASSIO%20NASCIMENTO&fontSize=46&fontColor=E5A93C&fontAlignY=42&desc=%E2%97%8F%20%20BACKEND%20.NET%20DEVELOPER%20%C2%B7%20PLENO%20%20%E2%97%8F&descSize=15&descAlignY=72&descColor=A39E93" width="100%" alt="Cassio Nascimento - Backend .NET Developer" />

  <br/>

  <!-- TAGS DE DESTAQUE IGUAIS AO HERO DO SITE -->
  <p align="center">
    <img src="https://img.shields.io/badge/C%23-1A1713?style=for-the-badge&logo=csharp&logoColor=E5A93C&labelColor=0F0D0B" alt="C#" />
    <img src="https://img.shields.io/badge/.NET%208-1A1713?style=for-the-badge&logo=dotnet&logoColor=E5A93C&labelColor=0F0D0B" alt=".NET 8" />
    <img src="https://img.shields.io/badge/ASP.NET%20Core-1A1713?style=for-the-badge&logo=dotnet&logoColor=E5A93C&labelColor=0F0D0B" alt="ASP.NET Core" />
    <img src="https://img.shields.io/badge/Clean%20Architecture-1A1713?style=for-the-badge&logoColor=E5A93C&labelColor=0F0D0B" alt="Clean Architecture" />
    <img src="https://img.shields.io/badge/DDD-1A1713?style=for-the-badge&logoColor=E5A93C&labelColor=0F0D0B" alt="DDD" />
    <img src="https://img.shields.io/badge/CQRS-1A1713?style=for-the-badge&logoColor=E5A93C&labelColor=0F0D0B" alt="CQRS" />
  </p>

  <!-- BIO CURTA DE IMPACTO -->
  <p align="center">
    <b>Construindo aplicações corporativas, APIs e arquiteturas backend com C#, .NET e engenharia de software orientada ao negócio.</b>
  </p>

  <!-- BOTÕES DE CONEXÃO RÁPIDA PARA RECRUTADORES -->
  <p align="center">
    <a href="https://www.linkedin.com/in/devcassio/">
      <img src="https://img.shields.io/badge/LinkedIn-Conectar-E5A93C?style=for-the-badge&logo=linkedin&logoColor=0F0D0B&labelColor=E5A93C" alt="LinkedIn" />
    </a>
    <a href="mailto:cassionascimentovieira@outlook.com">
      <img src="https://img.shields.io/badge/E--mail-Falar%20Comigo-1A1713?style=for-the-badge&logo=microsoftoutlook&logoColor=E5A93C&labelColor=1A1713" alt="Email" />
    </a>
  </p>

</div>

---

### `>//` Perfil & Engenharia de Software

Como desenvolvedor backend especializado no ecossistema **.NET**, meu foco é desenhar e construir sistemas corporativos escaláveis, resilientes e de fácil manutenção. Aplico **Clean Architecture**, **Domain-Driven Design (DDD)**, **CQRS** e princípios **SOLID** para isolar regras de negócio complexas de detalhes de infraestrutura, garantindo entregas seguras e testáveis.

```csharp
[ApiController]
[Route("api/v{version}/[controller]")]
public class ProfileController : ControllerBase
{
    private readonly ISender _mediator;

    public ProfileController(ISender mediator) => _mediator = mediator;

    [HttpGet("about-me")]
    public IActionResult GetProfile() => Ok(new 
    {
        Developer = "Cassio Nascimento",
        Role = "Backend .NET Developer Pleno",
        CoreStack = new[] { "C#", ".NET 8", "ASP.NET Core", "EF Core" },
        Architecture = new[] { "Clean Architecture", "DDD", "CQRS", "MediatR", "SOLID" },
        MessagingAndData = new[] { "SQL Server", "PostgreSQL", "Redis", "RabbitMQ", "Kafka" }
    });
}
