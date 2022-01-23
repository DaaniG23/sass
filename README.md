# sass

AGREGUE H1 EN EL INDEX,
H2 EN EL RESTO DE LAS PÁGINAS,
AGREGUÉ EN LA PÁG SUCURSALES UN MIXIN, EXTEND Y MAP-GET.
/* maps */
$colores: (
fondo: #dbca34,
letras: black,
);
/* agrego map-get */
.lachoppera {
	background: map-get($colores, fondo);
	.lacho {
		color: map-get($colores, letras);
		font-size: 30px;
		font-weight: bold;
		letter-spacing: 1px;
	}
	/* extend */
	.nave {
		.navegacion {
			font-size: 20px;
			color: $colorTexto;
			text-align: right;
		}
		.solo {
			@extend .navegacion;
		}
	}
  
  /* agrego mixin */
@mixin imagn {
	display: flex;
	flex-direction: row;
	align-items: center;
	flex-wrap: wrap;
}
#ubicaciones {
	div {
		@include imagn;
		margin-top: 20px;
		background-image: linear-gradient(to left, #dbca34, rgb(15, 14, 12));
	}
EN LA PAG SUCURSALES AGREGUÉ ESTAS KEYWORDS: cerveza, cerveceria, salidas, encuentros, amigos, bar, comida, villa crespo, puerto madero, palermo. Y ESTA DESCRIPCIÓN: Si buscas buena birra, estás buscando La Choppera Loca. Locales de estilo industrial, moderno y buen ambiente. Una gran opción para disfrutar con amigos, familia y pareja

EN LA PAG INDEX AGREGUÉ ESTAS KEYWORDS: cerveza, cerveceria, salidas, encuentros, amigos, juntada, bar, comida, papas fritas
Y ESTA DESCRIPCION: Si buscas buena birra, estás buscando La Choppera Loca. Locales de estilo industrial, moderno y buen ambiente. Una gran opción para disfrutar con amigos, familia y pareja.
