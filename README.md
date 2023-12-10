-- --------------------------------------------------------
-- Host:                         127.0.0.1
-- VersiÃ³n del servidor:         8.1.0 - MySQL Community Server - GPL
-- SO del servidor:              Win64
-- HeidiSQL VersiÃ³n:             12.5.0.6677
-- --------------------------------------------------------

/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET NAMES utf8 */;
/*!50503 SET NAMES utf8mb4 */;
/*!40103 SET @OLD_TIME_ZONE=@@TIME_ZONE */;
/*!40103 SET TIME_ZONE='+00:00' */;
/*!40014 SET @OLD_FOREIGN_KEY_CHECKS=@@FOREIGN_KEY_CHECKS, FOREIGN_KEY_CHECKS=0 */;
/*!40101 SET @OLD_SQL_MODE=@@SQL_MODE, SQL_MODE='NO_AUTO_VALUE_ON_ZERO' */;
/*!40111 SET @OLD_SQL_NOTES=@@SQL_NOTES, SQL_NOTES=0 */;


-- Volcando estructura de base de datos para integrador_cac
CREATE DATABASE IF NOT EXISTS `integrador_cac` /*!40100 DEFAULT CHARACTER SET latin1 COLLATE latin1_spanish_ci */ /*!80016 DEFAULT ENCRYPTION='N' */;
USE `integrador_cac`;

-- Volcando estructura para tabla integrador_cac.oradores
CREATE TABLE IF NOT EXISTS `oradores` (
  `id` int NOT NULL AUTO_INCREMENT,
  `nombre` varchar(40) CHARACTER SET latin1 COLLATE latin1_spanish_ci NOT NULL,
  `apellido` varchar(40) CHARACTER SET latin1 COLLATE latin1_spanish_ci NOT NULL,
  `mail` varchar(40) CHARACTER SET latin1 COLLATE latin1_spanish_ci NOT NULL,
  `tema` varchar(40) COLLATE latin1_spanish_ci NOT NULL,
  `fecha_alta` date NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `mail` (`mail`)
) ENGINE=InnoDB AUTO_INCREMENT=11 DEFAULT CHARSET=latin1 COLLATE=latin1_spanish_ci;

-- Volcando datos para la tabla integrador_cac.oradores: ~10 rows (aproximadamente)
INSERT INTO `oradores` (`id`, `nombre`, `apellido`, `mail`, `tema`, `fecha_alta`) VALUES
	(1, 'martin', 'arnedo', 'martinarnedo@gmail.com', 'tecnologia', '2023-12-10'),
	(2, 'maria', 'luna', 'maria12@gmail.com', 'clima', '2023-12-10'),
	(3, 'natalia', 'isnardi', 'nati@gmai.com', 'religion', '2023-11-23'),
	(4, 'eliana', 'maciel', 'eli@gmail.com\r\n', 'sociales', '2023-12-10'),
	(5, 'marcelo', 'lopez', 'marce@gmail.com', 'cultura', '2023-12-10'),
	(6, 'soledad', 'gomez', 'solegomez@gmail.com', 'economia', '2023-10-05'),
	(7, 'federico', 'sosa', 'fedesosa@gmail.com', 'viaje y turismo', '2023-01-25'),
	(8, 'patricio', 'vega', 'patovega@gmail.com', 'biologia', '2023-03-12'),
	(9, 'brisa', 'garcia', 'brisag@gmail.com', 'deportes', '2023-12-19'),
	(10, 'maria ', 'rojas', 'marirojas@gmail.com', 'quimica', '2023-04-18');

/*!40103 SET TIME_ZONE=IFNULL(@OLD_TIME_ZONE, 'system') */;
/*!40101 SET SQL_MODE=IFNULL(@OLD_SQL_MODE, '') */;
/*!40014 SET FOREIGN_KEY_CHECKS=IFNULL(@OLD_FOREIGN_KEY_CHECKS, 1) */;
/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40111 SET SQL_NOTES=IFNULL(@OLD_SQL_NOTES, 1) */;
