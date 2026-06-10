
using Microsoft.AspNetCore.Mvc;

namespace ProjetoMVC.Controllers
{
    public class HomeController : Controller
    {
        public IActionResult Index()
        {
            return View();
        }

        public IActionResult Sobre()
        {
            return View();
        }
    }
}

@{
    ViewData["Title"] = "Sobre";
}

<h1>Sobre o Projeto</h1>

<p>Projeto desenvolvido para a disciplina de Desenvolvimento Web.</p>

<p>Utilizando ASP.NET MVC, Controllers, Views, Rotas e Tag Helpers.</p>

<p>Autor: Aluno</p>

<!DOCTYPE html>
<html>
<head>
    <title>Projeto MVC</title>
</head>
<body>
    <nav>
        <a asp-controller="Home" asp-action="Index">Home</a> |
        <a asp-controller="Aluno" asp-action="Index">Alunos</a> |
        <a asp-controller="Home" asp-action="Sobre">Sobre</a>
    </nav>

    <div>
        @RenderBody()
    </div>
</body>
</html>
