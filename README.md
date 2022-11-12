SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";

CREATE TABLE `person` (
  `Id` int(11) NOT NULL,
  `Name` varchar(20) DEFAULT NULL,
  `Surname` varchar(30) DEFAULT NULL,
  `City` varchar(40) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

INSERT INTO `person` (`Id`, `Name`, `Surname`, `City`) VALUES
(1, 'Kamil', 'Kłobukowski', 'Warszawa'),
(2, 'Jan', 'Kowalski', 'Kraków'),
(3, 'Adam', 'Nowak', 'Poznań');

ALTER TABLE `person`
  ADD PRIMARY KEY (`Id`);
COMMIT;
