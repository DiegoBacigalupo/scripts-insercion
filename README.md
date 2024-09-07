# scripts-insercion

use formulauno;
-- Datos de ejemplo para Driver_Championships
INSERT INTO `Driver_Championships` (`id_driver`, `year`, `championship_type`, `position`) VALUES
(1, 2023, 'World Championship', 1),
(2, 2023, 'World Championship', 2),
(3, 2022, 'World Championship', 3);

-- Datos de ejemplo para Team_Championships
INSERT INTO `Team_Championships` (`id_team`, `year`, `championship_type`, `position`) VALUES
(1, 2023, 'Constructors Championship', 1),
(2, 2023, 'Constructors Championship', 2),
(3, 2022, 'Constructors Championship', 3);

-- Datos de ejemplo para Race_Results
INSERT INTO `Race_Results` (`id_grandprix`, `id_driver`, `id_team`, `position`, `points`) VALUES
(1, 1, 1, 1, 25.0),
(1, 2, 1, 2, 18.0),
(2, 3, 2, 1, 25.0);

-- Datos de ejemplo para Driver_Standings
INSERT INTO `Driver_Standings` (`year`, `id_driver`, `id_team`, `points`) VALUES
(2023, 1, 1, 300.0),
(2023, 2, 1, 250.0),
(2022, 3, 2, 275.0);

-- Datos de ejemplo para Team_Standings
INSERT INTO `Team_Standings` (`year`, `id_team`, `points`) VALUES
(2023, 1, 550.0),
(2023, 2, 300.0),
(2022, 3, 400.0);

-- Datos de ejemplo para Track_Records
INSERT INTO `Track_Records` (`id_grandprix`, `id_driver`, `id_team`, `lap_time`) VALUES
(1, 1, 1, '01:30:45'),
(2, 2, 1, '01:31:20'),
(1, 3, 2, '01:32:10');

-- Datos de ejemplo para Pit_Stops
INSERT INTO `Pit_Stops` (`id_grandprix`, `id_driver`, `id_team`, `stop_number`, `stop_duration`) VALUES
(1, 1, 1, 1, '00:02:30'),
(1, 2, 1, 2, '00:02:45'),
(2, 3, 2, 1, '00:03:00');
